# SigmaOS Browser Handoff

A Rust state model for browser selection and URL handoff. `BrowserHandoff` tracks a default or custom browser, records deferred URLs when no browser is configured, exposes handoff outcomes, and includes URL-host extraction helpers.

The current library reports which browser should handle a URL; it does not launch a browser process or integrate with desktop URL handlers. Deferred URLs are in-memory state and are not persisted.

## Build

The manifest references sibling [`SigmaOS-kernel`](../SigmaOS-kernel). From the SigmaOS checkout:

```sh
cargo check --manifest-path SigmaOS-browser-handoff/Cargo.toml --lib
```

## License

GPL-3.0-or-later. See [`Cargo.toml`](Cargo.toml).
