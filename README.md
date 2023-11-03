# Ghalias

Managed list of GitHub CLI aliases

## Summary

Essential goal of Ghalias is to turns [GitHub CLI](https://cli.github.com/manual/gh) command into shortest possible sequence of characters where the alias does not have to be remembered but it can be mnemotechnically derived from the full command.

## Usage

Import list of aliases to your GitHub CLI config file:

```sh
curl https://raw.githubusercontent.com/josefpihrt/ghalias/main/config.yml | gh alias import -
```

Alternatively, overwrite existing aliases:

```sh
curl https://raw.githubusercontent.com/josefpihrt/ghalias/main/config.yml | gh alias import --clobber -
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
