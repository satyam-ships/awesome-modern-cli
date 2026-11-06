# awesome-modern-cli ⌨️

> Faster, friendlier replacements for classic Unix tools, and the one-liners that make them click.

| Classic | Modern | What you get | Install (macOS) |
|---|---|---|---|
| `grep` | [ripgrep](https://github.com/BurntSushi/ripgrep) `rg` | Fast, respects .gitignore | `brew install ripgrep` |
| `find` | [fd](https://github.com/sharkdp/fd) | Simple syntax, fast | `brew install fd` |
| `cat` | [bat](https://github.com/sharkdp/bat) | Syntax highlighting | `brew install bat` |
| `ls` | [eza](https://github.com/eza-community/eza) | Icons, git status | `brew install eza` |
| `cd` | [zoxide](https://github.com/ajeetdsouza/zoxide) | Jump to frequent dirs | `brew install zoxide` |
| `man` | [tldr](https://github.com/tldr-pages/tldr) | Practical examples | `brew install tldr` |
| `diff` | [delta](https://github.com/dandavison/delta) | Readable diffs | `brew install git-delta` |
| `top` | [btop](https://github.com/aristocratos/btop) | Rich system monitor | `brew install btop` |
| `curl` | [httpie](https://github.com/httpie/cli) | Human-friendly HTTP | `brew install httpie` |
| `sed`/JSON | [jq](https://github.com/jqlang/jq) | Query JSON | `brew install jq` |
| fuzzy anything | [fzf](https://github.com/junegunn/fzf) | Fuzzy finder | `brew install fzf` |
| `du` | [dust](https://github.com/bootandy/dust) | Visual disk usage | `brew install dust` |

## Power one-liners
```bash
rg -n "TODO" --glob '!node_modules'          # search code
fd -e log -x rm {}                            # delete all .log files
git log --oneline | fzf --preview 'git show {1}'   # browse commits
curl -s api.example.com/users | jq '.[].email'     # extract fields
z proj                                        # jump to ~/work/projects
```

## Contributing
Add a tool with: what it replaces, why it's better, install command. License [MIT](LICENSE).
