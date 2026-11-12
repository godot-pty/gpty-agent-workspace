# gpty-agent-workspace

The Agent Workspace layout for [gpty](https://github.com/godot-pty/gpty) — a gpty plugin shipping one profile: a wide agent terminal with the Inspector and Reasoning panes stacked beside it.

## Install

    gpty plugin install godot-pty/gpty-agent-workspace

Installation clones this repo, validates `gpty-plugin.toml` with the shipped validator, and asks a human to review it in the gpty GUI before anything installs — a plugin's content runs as you, so acceptance is explicit and pinned to the revision you reviewed. A newer revision asks again.

## Layout

- **Agent Workspace** — an `omp-terminal` terminal on the left, and Inspector (OMP-backed) and Reasoning panes on the right. The Reasoning pane follows the terminal by its stable attachment id.

The app ships the same layout as a seeded default on a fresh install. Installing this plugin while that copy exists asks to replace it; confirming gives the name to the plugin-owned copy, which can then be uninstalled from its sidebar trash.

The profile names no program, so activation does not raise a Workspace Trust dialog. The Inspector's `omp` backend observes an OMP session in the terminal.
