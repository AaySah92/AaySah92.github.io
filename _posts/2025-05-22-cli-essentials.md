---
title: "CLI Essentials"
date: 2025-05-22
---
I have been using Linux on my personal laptop since 2012. And over the years, I have grown more and more comfortable with the command-line interface (CLI). It was a great feeling in the early years when I'd ***UPDATE*** my Fedora Workstation (I remember I started with Fedora 16). That was the only time, I would open the terminal. And I loved it. Well... that and when I would break my installation and Stack Overflow would tell me to run `<this command>` in the terminal.

Reinstalling GRUB made me feel like a hacker. 😅

But it was when I started working on servers that I really got into CLI. Managing multiple LAMP stack servers can really taught me a thing or two. Over the years, I’ve discovered some amazing tools that have made my life so much easier—so much so, I ’ve started using them on my personal laptop too.

Let me share some of these here and show you how they help make my workflow smooth.

### BAT - [https://github.com/sharkdp/bat](https://github.com/sharkdp/bat)
`bat` is a replacement for the `less` command. It's got syntax highlighting and git integrations. It makes it so much easier to read the contents of a file compared to `less`.

| Here's a comparison - Reading a TOML file. |
| -- |
| `LESS` |
| ![less](/assets/images/cli-essentials/less.png) | 
| `BAT` |
| ![bat](/assets/images/cli-essentials/bat.png) |

### FD - [https://github.com/sharkdp/fd](https://github.com/sharkdp/fd)
`fd` is a replacement for `find`, but it's faster and more intuitive. Let's say you want to find a config file in the /etc directory and you only know part of the name. You'd run something like `find /etc -iname '*httpd*'`(`-i` makes the search case-insensitive). With `fd`, it would be as simple as `fd http /etc`. It might not look much, but when you're constantly working on servers, it saves you a couple of keystrokes.

On top of that, `fd` respects the `.gitignore` entries. So if you were looking for a `.ts` file in your project and you have an entry in the `.gitignore` to exclude the `node_modules` directory, it won't list results from `node_modules`. Isn't that great?

| Here's a comparison - Finding *my* tmux config file. |
| -- |
| `FIND` - it's the last one in the long list. |
| ![find](/assets/images/cli-essentials/find.png) | 
| `FD` |
| ![fd](/assets/images/cli-essentials/fd.png) |

