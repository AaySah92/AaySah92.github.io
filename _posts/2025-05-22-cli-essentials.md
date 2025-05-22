---
title: "CLI Essentials"
date: 2025-05-22
---
I have been using Linux on my personal laptop since 2012. And over the years, I have grown more and more comfortable with the command-line interface (CLI). It was a great feeling in the early years when I'd ***UPDATE*** my Fedora Workstation (I remember I started with Fedora 16). That was the only time, I would open the terminal. And I loved it. Well... that and when I would break my installation and Stack Overflow would tell me to run `<this command>` in the terminal.

Reinstalling GRUB made me feel like a hacker. 😅

But it was when I started working on servers that I really got into CLI. Managing multiple LAMP stack servers can really taught me a thing or two. Over the years, I’ve discovered some amazing tools that have made my life so much easier—so much so, I ’ve started using them on my personal laptop too.

Let me share some of these here and show you how they help make my workflow smooth.

### BAT
`bat` is a replacement for the `less` command. It's got syntax highlighting and git integrations. It makes it so much easier to read the contents of a file compared to `less`.
Here's a comparison.

#### Reading a TOML file with `less`
![less](/assets/images/cli-essentials/less.png)

#### Reading the same TOML file with `bat`
![bat](/assets/images/cli-essentials/bat.png)

Github link: https://github.com/sharkdp/bat

### FD
`fd` is a replacement for `find`.
