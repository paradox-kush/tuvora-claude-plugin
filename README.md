# Tuvora for Claude Code

Connects Claude Code to your [Tuvora](https://tuvora.co) account so you can manage it in plain words: "hide the adult channels", "make a Sports group with my football channels", "which of my add-ons are broken?". Every change is previewed first and saved only when you confirm. Changes sync to your Tuvora apps.

## Install

```
/plugin marketplace add paradox-kush/tuvora-claude-plugin
/plugin install tuvora@tuvora
```

Then run `/mcp`, pick **tuvora**, and sign in to Tuvora when the browser opens. Tap **Allow** on the consent screen.

### Only in the projects that need it

Claude Code connects to every enabled plugin's server at the start of **every** session, including `claude -p` runs and scripts, even when you never ask about Tuvora. If you start Claude Code a lot, install it for one project instead of for all of them:

```
claude plugin install tuvora@tuvora --scope local
```

Run that inside the project folder. `--scope local` is just for you; `--scope project` shares it with everyone who uses the repository.

Already installed everywhere? Turn it off in projects that don't need it with `claude plugin disable tuvora@tuvora --scope local`, or switch the server off in `/mcp`.

## What it can do

- **Account:** profiles and devices, rename a device.
- **Playlists:** list, refresh, rename, turn on or off, reorder, delete; check guide coverage.
- **Live TV:** list categories and groups, search channels, find duplicate channels, preview and apply changes (hide, show, pin, reorder, custom groups), delete a group, reset customisation.
- **Favourites and Home:** list and change favourites, see and rearrange the Home rows.
- **Add-ons:** list add-ons and run a health check.

Live TV editing and guide coverage work for Xtream playlists. The full list is at https://tuvora.co/ai-assistants.

## What it can't do

See or change playlist addresses, usernames or passwords; change profile PINs; sign devices out; delete your account.

## Privacy and support

- Docs: https://tuvora.co/ai-assistants
- Privacy: https://tuvora.co/privacy#ai-assistants
- Disconnect any time under Account, Devices, Connected assistants at tuvora.co.
- Support: rockkevin47@gmail.com

MIT licensed.
