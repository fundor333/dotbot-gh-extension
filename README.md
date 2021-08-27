# dotbot-gh-extension
Plugin for DotBot for GH Extension

Plugin for [`dotbot`](https://github.com/anishathalye/dotbot) to edit and sync crontab without deleting or editing manual added cronjob, only manage dotbot cron.

## Installation

1. Add `dotbot-gh-extension` as a submodule of your dotfiles repository.

```bash
git submodule add https://github.com/fundor333/dotbot-gh-extension.git
```

2. Modify your `install` script to enable the `dotbot-gh-extension` plugin.

```bash
"${BASEDIR}/${DOTBOT_DIR}/${DOTBOT_BIN}" -d "${BASEDIR}" --plugin-dir dotbot-gh-extension -c "${CONFIG}" "${@}"
```

## Usage

The plugin adds one directive use with `ghe` with the repo. 

For example:



```yaml
- ghe:
  - vilmibm/gh-screensaver
  - vilmibm/gh-user-status
  - samcoe/gh-triage
```
