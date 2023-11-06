# GH Joe

## Summary

GH Joe is a managed list of [GitHub CLI](https://cli.github.com/manual/gh) [aliases](https://cli.github.com/manual/gh_alias).

Main idea is that each command should be represented by shortest possible sequence of characters (an alias) where the alias does not have to be remembered but it can be mnemotechnically derived from the full command.

For a full list of aliases please see [config.yml](https://github.com/josefpihrt/ghjoe/blob/main/config.yml).

## Installation

Import list of aliases to your GitHub CLI config file:

```sh
curl https://raw.githubusercontent.com/josefpihrt/ghjoe/main/config.yml | gh alias import -
```

Optionally, overwrite existing aliases:

```sh
curl https://raw.githubusercontent.com/josefpihrt/ghjoe/main/config.yml | gh alias import --clobber -
```

## Commands Aliases

| Alias | Command |
| --- | --- |
| `a` | `alias` |
| `b` | `browse` |
| `c` | `codespace` |
| `e` | `release` |
| `g` | `gist` |
| `h` | `auth` |
| `i` | `issue` |
| `j` | `project` |
| `k` | `cache` |
| `l` | `label` |
| `n` | `run` |
| `o` | `config` |
| `p` | `pr` |
| `r` | `repo` |
| `s` | `search` |
| `t` | `secret` |
| `u` | `status` |
| `v` | `variable` |
| `w` | `workflow` |
| `x` | `extension` |

## Aliases Creation Rules

Each alias is created according to several simple rules:

1. **Each root command is represented by a single letter.**
   - For example `issue`  is represented by `i`.

2. **Each subcommand/parameter/value is represented by combination of first letter of words it consists of.**
   - For example subcommand `release delete-asset` is represented by `rda`.
   - For example parameter `--exclude-pre-releases` is represented by `epr`.

3. **Parameters are sorted in alphabetical order.**
   - For example command `pr create --assignee @me --draft --title` is represented by `pcamdt`.