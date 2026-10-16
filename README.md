# Awesome-Command-Line-Navigation

# Top Command Line Navigation Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Directory Jumping, Fuzzy Finding & Shell History Search*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Command Line Navigation**. These tools enable developers to move through the filesystem at the speed of thought—jumping to directories by remembered keywords instead of typing paths, fuzzy-finding files interactively, and searching shell history across sessions and machines.

**Examples** include zoxide, fzf, autojump, fasd, z, broot, Atuin, McFly, Jump, and Yazi (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for shell integration, fuzzy matching, and history search—ideal for developers, sysadmins, and anyone who lives in the terminal.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **Terminal Emulators with Built-in Navigation** (Warp, iTerm2, Windows Terminal)  
  Some terminal emulators now ship with directory bookmarks, autocompletion, and AI-assisted navigation as built-in features, reducing the need for standalone tools.

## Open-Source GitHub Projects

- **[zoxide](https://github.com/ajeetdsouza/zoxide)**  
  **A smarter, faster `cd` command that tracks your most used directories** (MIT) . **36,752+ GitHub stars** . **The modern standard for directory jumping**—**inspired by `z` and autojump, reimplemented in Rust for speed and cross-shell consistency** . **Frecency algorithm** ranks directories by frequency and recency, so it learns your habits and gets more accurate over time . **Startup time: ~5 ms** vs. autojump's ~50 ms and fasd's ~20 ms . **Query time: <10 ms** across 10,000 tracked directories . **Import from other tools**: `zoxide import autojump`, `zoxide import fasd`, `zoxide import z`, `zoxide import atuin` . **Supports 9+ shells**: Bash, Zsh, Fish, Nushell, PowerShell, Elvish, Tcsh, Xonsh, and POSIX . **Native Windows support** via winget, Scoop, Chocolatey, and Cargo . **`zi` opens an fzf-powered interactive menu** when multiple matches exist—type a few characters, select, jump . **SQLite database** for history storage . **The reference implementation for directory jumping** .

- **[fzf](https://github.com/junegunn/fzf)**  
  **A command-line fuzzy finder** (MIT) . **The most powerful general-purpose fuzzy finder**—**matches files, command history, processes, hostnames, bookmarks, git commits, and more** . **Powers zoxide's interactive `zi` mode** . **Key bindings for CTRL-T (files), CTRL-R (history), and ALT-C (cd)** . **`--scheme=path`** for file paths, **`--scheme=history`** for chronological data . **Shell integration for Bash, Zsh, and Fish** . **Vim/Neovim plugin** available . **The most widely adopted fuzzy finder in the terminal ecosystem** .

- **[Atuin](https://github.com/atuinsh/atuin)**  
  **Magical shell history** (MIT) . **Replaces your existing shell history with a SQLite database** and records **additional context**—exit code, working directory, hostname, session, command duration . **Back up and sync encrypted shell history** across machines . **Full-screen history search UI** bound to Ctrl-r and up . **Filter modes**: search history from the current session, current directory, or globally . **Quick-jump to previous items with Alt-<num>** . **Statistics** like "most used command" . **Note**: Bash users need `ble.sh` or `bash-preexec` . **The emerging standard for shell history search** .

- **[autojump](https://github.com/wting/autojump)**  
  **A `cd` command that learns** (GPL-3.0) . **16,304+ GitHub stars** . **The classic directory jumper**—**one of the oldest tools in the category** . **Widely packaged** in Linux distributions . **Limitations**: Python-based (slower startup), prefix-only matching (no fuzzy search), and low active maintenance . **zoxide supports importing autojump data** for migration . **Best for**: environments where autojump is already standardized and working .

- **[fasd](https://github.com/clvv/fasd)**  
  **Command-line productivity booster, offers quick access to files and directories** (MIT) . **Ranks files AND directories**, not just directories . **Supports "jump + open file" workflows** . **POSIX sh-based** with partial fuzzy search . **Stalled maintenance** . **Best for**: users who want directory jumping and file opening in one tool .

- **[z (rupa/z)](https://github.com/rupa/z)**  
  **Jump around** (WTFPL) . **16,390+ GitHub stars** . **The original lightweight `z` script**—minimal dependencies, simple shell script . **Fragmented ecosystem** with many forks and feature differences . **zoxide is explicitly inspired by `z` and modernizes the concept** . **Best for**: minimalists who want a simple script and don't need cross-shell consistency .

- **[broot](https://github.com/Canop/broot)**  
  **Tree view, file manager, configurable launcher** (MIT) . **The most feature-rich terminal file navigator**—**displays directory contents in a tree-like view, lets you filter using fuzzy patterns and regex, and integrates with git to hide ignored files by default** . **Preview files and images** in high resolution if the terminal supports Kitty's graphics protocol . **Launch actions and define custom shortcuts** . **Best for**: developers who want visual tree navigation without leaving the terminal .

- **[Yazi](https://github.com/sxyazi/yazi)**  
  **Blazing fast terminal file manager written in Rust** (MIT) . **The modern Ranger replacement**—**terminal-based file manager for rapid filesystem browsing** . **Vim-like keybindings** . **Best for**: users who want a full TUI file manager rather than just directory jumping .

- **[McFly](https://github.com/cantino/mcfly)**  
  **Fly through your shell history** (MIT) . **The neural-network-powered history search**—**uses a small neural network to rank history suggestions based on context** . **Replaces Ctrl-r with a smarter search** . **Best for**: users who want history search that learns from context .

- **[Jump](https://github.com/gsamokovarov/jump)**  
  **Jump helps you navigate faster by learning your habits** (MIT) . **1,801+ GitHub stars** . **The Go-based directory jumper**—**simpler than zoxide, focused on directory history** . **Best for**: Go users who want a single-binary directory jumper .

- **[z.lua](https://github.com/skywind3000/z.lua)**  
  **A new cd command that helps you navigate faster by learning your habits** (MIT) . **The Lua-based directory jumper**—**extremely fast and highly configurable** . **Best for**: Neovim-heavy users already in the Lua ecosystem who want maximum customization .

### Additional Strong Open-Source Options

- **[skim](https://github.com/skim-rs/skim)** — Fuzzy finder in Rust (MIT) . **5,219+ GitHub stars** . **The Rust alternative to fzf**—fzf-compatible options, async execution, and ~3.9MB binary . **Best for**: Rust users who want a fzf alternative with modern architecture .
- **[peco](https://github.com/peco/peco)** — Simplistic interactive filtering tool (MIT) . **7,697+ GitHub stars** . **The original Go fuzzy finder**—simpler than fzf but widely used .
- **[fzf-marks](https://github.com/urbainvaes/fzf-marks)** — Bash/Zsh plugin for managing bookmarks with fzf (MIT) . **Alternative workflow to zoxide** for explicit bookmark management .
- **[zsh-vi-mode](https://github.com/jeffreytse/zsh-vi-mode)** — Proper Vim mode for Zsh (MIT) . **Improves terminal navigation with Vim keybindings** .
- **[fast-syntax-highlighting](https://github.com/zdharma-continuum/fast-syntax-highlighting)** — While-you-type syntax highlighting (BSD-3-Clause) . **Makes command feedback visual** .
- Community **n8n** workflows for dotfiles synchronization and shell configuration automation.

**Frameworks for building custom systems**: Combine **zoxide** for directory jumping with **fzf** for interactive selection, **Atuin** for history search across machines, and **broot** for visual tree navigation—creating a comprehensive terminal navigation stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Command line navigation tools handling shell history and directory paths must follow security best practices, especially when syncing history across machines.
- **Open-source navigation tools are mature and production-ready.** zoxide is the modern default with 36K+ stars and ~5ms startup . fzf is the most widely adopted fuzzy finder . Atuin brings SQLite-backed history search with encrypted sync . **These are genuine alternatives to native `cd` and shell history** .
- **zoxide vs. autojump: the migration is easy.** zoxide supports importing autojump, fasd, z, and Atuin databases . Startup time is ~10x faster than autojump . **If you're still on autojump, migrate to zoxide** .
- **The "learns your habits" distinction is the core value.** `cd` requires you to know the path. zoxide, autojump, and fasd require you to remember **intent**—type a few letters, and the tool finds the most "frecent" match . **This shifts navigation from path-recall to keyword-recall** .
- **fzf is the integration layer.** zoxide's interactive mode depends on fzf . fzf can fuzzy-find files, history, processes, and git commits . **Install fzf regardless of which directory jumper you choose** .
- **History search is the unsung hero.** Atuin replaces Ctrl-r with a searchable, syncable, context-rich history database . **Finding that command you ran three weeks ago in a specific directory becomes instant** .
- Self-hosted open-source solutions require proper shell configuration and database management. **Navigation tools are deeply personal**—invest time in your setup and it pays dividends every day.

---

**Made for developers, sysadmins, and anyone who lives in the terminal.**  
Let's make Command Line Navigation more open, data-driven, and instant.
