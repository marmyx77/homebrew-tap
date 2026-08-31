# marmyx77/homebrew-tap

Homebrew casks published from this account.

```sh
brew tap marmyx77/tap
brew trust marmyx77/tap
brew install --cask lampboard
```

Since Homebrew 6 a cask from a third-party tap is refused until the tap is
trusted. Without the middle line the install ends at *Refusing to load cask …
from untrusted tap*, which names neither the cask nor anything a newcomer can
act on.

**[LampBoard](https://github.com/marmyx77/lampboard)** — a floating column of
traffic lights that tells you, at a glance, what state your coding sessions are
in: Claude Code and Codex, in VS Code, in a terminal, in a desktop app, on
another machine.

The cask is rendered by `Scripts/make-cask.sh` in that repository, from a
published release: the checksum is taken from the asset GitHub serves, never
from a local build, because a checksum read locally is right on the machine
cutting the release and wrong for everybody else the moment a rebuild differs by
a byte.
