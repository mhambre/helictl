# Helictl - Helios Control

`helictl` is the control-plane CLI for Helios. It is intended to talk to a running `helid` instance and provide operator-facing control commands.

For top-level build scripts, shared targets, and project-wide setup, use the main Helios README:  
https://github.com/mhambre/helios

## Build / Run / Debug

From the Helios monorepo root:

```bash
just build control release
just build control debug
just gdb control
```

Direct cargo build:

```bash
cargo +nightly build -p helictl --target x86_64-unknown-linux-gnu
```

Run directly after build:

```bash
./target/x86_64-unknown-linux-gnu/debug/helictl
```
