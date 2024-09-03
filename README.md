# workshop-prerequisites

In order to ensure a smooth workshop experience for all attendees, We ask you to setup and install the tools needed for the duration of the workshop.

Operating systems supported: Windows, Mac, Linux
Time needed: ~10 minutes

### Git and Rust

First, We should check if Git and Rust are installed. Run these commands and if the output was successful, Move on to the next step.
```
git --version
cargo --version
```

If the above commands are not working, Try installing Git and Rust from the below links:

- Install [Git](https://git-scm.com/downloads)
- Install [Rust](https://www.rust-lang.org/tools/install)

### Rust on windows
Rust runs on many platforms, and there are many ways to install Rust. This guide describes installation via rustup, a tool that manages multiple Rust toolchains in a consistent way across all platforms Rust supports.
- On Windows, download and run [rustup-init.exe](https://static.rust-lang.org/rustup/dist/i686-pc-windows-gnu/rustup-init.exe)
- rustup-init can be configured interactively, and all options can additionally be controlled by command-line arguments, which can be passed through the shell script. Pass --help to rustup-init as follows to display the arguments rustup-init accepts:
```
    curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- --help
```
- The above command needs to executed using WSL
- If you prefer not to use the shell script, you may directly download rustup-init for windows [here](https://static.rust-lang.org/rustup/dist/x86_64-pc-windows-msvc/rustup-init.exe)
- Verify rust installation by running ```rustc --version``` in wsl

## Installing Leo

Check if you have leo installed by running this command in your terminal/command prompt

```
leo --version
```

If this command resulted in errors, or if the leo version is smaller than 2.0.0, Run this command:

```
# Download the source code
git clone https://github.com/ProvableHQ/leo
cd leo
git checkout testnet-beta
```

And then, build and install leo using the command below. This could take a few minutes depending on your machine.

```
cargo install --path .
```

If that was successful, run the version command again and if it showed a version, move on to the next step.

## Troubleshooting
If there was any issues installing these tools, you can ask for help in Aleo's official [Discord server](https://discord.gg/aleo)