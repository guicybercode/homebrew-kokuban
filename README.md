# Homebrew tap for Kokuban

[Kokuban](https://github.com/guicybercode/kokuban.rs) is a native Rust terminal for Linux and macOS.

```sh
brew tap guicybercode/kokuban
brew trust guicybercode/kokuban      # Homebrew 7 loads third-party taps only after this
brew install kokuban.rs              # `kokuban` executable: macOS (Apple Silicon, Intel) and Linux x86_64
brew install --cask kokuban          # Kokuban.app in /Applications (macOS)
```

Upgrade with `brew upgrade kokuban.rs` or `brew upgrade --cask kokuban`, not with `kokuban --update`.

Both packages install the files published on the
[GitHub releases](https://github.com/guicybercode/kokuban.rs/releases) and check them against
the published SHA-256. They are generated from
[`packaging/homebrew/`](https://github.com/guicybercode/kokuban.rs/tree/main/packaging/homebrew)
in the main repository by `scripts/update-homebrew.sh`; do not edit them here.

In a `brew bundle` `Brewfile`:

```ruby
tap "guicybercode/kokuban"
brew "kokuban.rs"
cask "kokuban"
```
