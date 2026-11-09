# cmdai-hq Homebrew tap

Homebrew formulae for [cmdai-hq](https://github.com/cmdai-hq) projects.

## Busy Crew

[Busy Crew](https://github.com/cmdai-hq/busy-crew) shows your Claude Code and Codex sessions on a BUSY Bar's LED display. macOS only.

```sh
brew install cmdai-hq/tap/busy-crew
busy-crew install --address http://busybar.local --timezone Europe/Paris
```

After `brew upgrade busy-crew`, run `busy-crew install` again: it keeps your settings and restarts the collector. Before `brew uninstall busy-crew`, run `busy-crew uninstall`, which removes its LaunchAgents and Claude Code hooks; Homebrew cannot do this for you.

Report problems with Busy Crew itself in [its repository](https://github.com/cmdai-hq/busy-crew/issues), and problems with the formula here.

## Humanload (closed beta)

Humanload counts, on your Mac, the work of supervising coding agents in Claude Code, and sends only those counts to
`app.humanload.eu`. The beta is by invitation; macOS 13 or later.

```sh
brew install cmdai-hq/tap/humanload
humanload setup
humanload login
```

Updates come only through `brew upgrade humanload`. Before `brew uninstall humanload`, run `humanload uninstall`: it
revokes the Mac and removes the Claude Code hooks, the two LaunchAgents and the Keychain key; Homebrew cannot. The beta
build is ad hoc signed, not by an identified developer. Testers receive the full guide with their invitation and report
problems to Tristan directly.
