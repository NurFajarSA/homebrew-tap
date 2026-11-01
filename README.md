# NurFajarSA Homebrew tap

Homebrew casks for [Accounts Manager for Claude](https://github.com/NurFajarSA/claude-switch), a menu bar app and CLI (`cs`) that runs several Claude accounts on one Mac and moves your work to the account with the most usage left.

```bash
brew install --cask nurfajarsa/tap/accounts-manager-for-claude
cs install --app "/Applications/Accounts Manager for Claude.app"
```

`cs install` sets up the background poller, the MCP server and the Claude Code hooks. Run it again after `brew upgrade`. Before `brew uninstall`, run `cs uninstall`.

Releases are ad-hoc signed until the project has an Apple Developer ID, so the cask clears the quarantine flag after installing. See the [install notes](https://github.com/NurFajarSA/claude-switch#install) for details.

Requires macOS 15 or later on Apple silicon.

## VM Manager

[VM Manager](https://github.com/NurFajarSA/vm-manager) keeps your SSH servers in one list, opens a shell on any of them from the menu bar, and lets Claude work on them through an MCP server that asks you before changing production.

```bash
brew install --cask nurfajarsa/tap/vm-manager
vm install --app "/Applications/VM Manager.app"
```
