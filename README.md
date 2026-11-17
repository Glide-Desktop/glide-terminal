# Glide Terminal

The terminal of the [Glide desktop](https://github.com/Glide-Desktop), built on
`alacritty_terminal`: tabs and splits, profiles, find, marks, URL hints, root
and SSH badges.

## Build

```sh
cargo build --release
```

The shared crates come from a tag of
[glide-libs](https://github.com/Glide-Desktop/glide-libs). To build against a
checkout of glide-libs next to this one, create `.cargo/config.toml` (ignored
by git):

```toml
[patch."https://github.com/Glide-Desktop/glide-libs"]
glide-app = { path = "../glide-libs/crates/glide-app" }
glide-config = { path = "../glide-libs/crates/glide-config" }
glide-sdk = { path = "../glide-libs/crates/glide-sdk" }
```

Split from the Glide monorepo with its history in November 2026.
