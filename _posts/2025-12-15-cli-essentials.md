---
title: "CLI Essentials"
layout: post
tags:
   - Linux
   - CLI
   - BAT
   - FD
   - LSD
   - FZF
   - TMUX
---

I have been using Linux on my personal laptop since 2012. And over the years, I have grown more and more comfortable with the command-line interface (CLI). It was a great feeling in the early years when I'd ***UPDATE*** my Fedora Workstation (I remember I started with Fedora 16). That was the only time, I would open the terminal. And I loved it. Well... that and when I would break my installation and Stack Overflow would tell me to run `<this command>` in the terminal.

Reinstalling GRUB made me feel like a hacker. 😅

But it was when I started working on servers that I really got into CLI. Managing multiple LAMP stack servers can really teach you a thing or two. Over the years, I’ve discovered some amazing tools that have made my life so much easier that I ’ve started using them on my personal laptop too.

Let me share some of these here and show you how they help make my workflow smooth.

### BAT

`bat` is a replacement for the `less` command. It's got syntax highlighting and git integrations. It makes it so much easier to read the contents of a file compared to `less`.

<iframe
   src="https://www.youtube.com/embed/C3BqKmd8lJQ"
   style="width:100%;aspect-ratio:16/9;"
   frameborder="0"
   allowfullscreen>
</iframe>

<a href="https://github.com/sharkdp/bat" target="_blank" rel="noopener noreferrer">
View source on GitHub ↗
</a>

---

### FD

`fd` is a replacement for `find`, but it's faster and more intuitive. 

Let's say you want to find a config file in the /etc directory, and you only know part of the name. You'd run something like `find /etc -iname '*httpd*'`. With `fd`, it would be as simple as `fd http /etc`. It might not look much, but when you're constantly working on servers, it saves you a couple of keystrokes.

On top of that, `fd` respects the `.gitignore` entries. Isn't that great? Let me show you what I mean. I'll search for my tmux config file in my git repo which has other config files that are present in `.gitignore`.

<iframe
   src="https://www.youtube.com/embed/PgCNYR2PmIk"
   style="width:100%;aspect-ratio:16/9;"
   frameborder="0"
   allowfullscreen>
</iframe>

<a href="https://github.com/sharkdp/fd" target="_blank" rel="noopener noreferrer">
View source on GitHub ↗
</a>

---

### LSD

`lsd` is a replacement for `ls` with colors and icons for different type of files and directories. This alone is a big step up from `ls` because it makes the output much more readable. You can also customize the output as much as you want since, just like other tools in this list, it's configurable. Plus it has themes if you like to style your terminal. 

I use it so often that I've *aliased* `ls` to `lsd` in my Bash config.

<iframe
   src="https://www.youtube.com/embed/dNflbIRMq9s"
   style="width:100%;aspect-ratio:16/9;"
   frameborder="0"
   allowfullscreen>
</iframe>

<a href="https://github.com/lsd-rs/lsd" target="_blank" rel="noopener noreferrer">
View source on GitHub ↗
</a>

---

### FZF

`fzf` is a fuzzy finder application that is used by many applications. It's basically used to find something based on your input. The shell integrations in particular have made my life so much easier. Let me show you how:

`CTRL-T` - Using this, you can search for a file *while* typing a command, and it will insert the path of the selected file in place. 

<iframe
   src="https://www.youtube.com/embed/Zs6JXlrtxZI"
   style="width:100%;aspect-ratio:16/9;"
   frameborder="0"
   allowfullscreen>
</iframe>

`CTRL-R` - Using this, you can go through your command history. And as you type, they get filtered. Once, you select a command, it's pasted on the command line.

<iframe
   src="https://www.youtube.com/embed/SC7gmwUO3KE"
   style="width:100%;aspect-ratio:16/9;"
   frameborder="0"
   allowfullscreen>
</iframe>

`ALT-C` - Using this, you can cd into the selected directory.

<iframe
   src="https://www.youtube.com/embed/G4R8vRA3_js"
   style="width:100%;aspect-ratio:16/9;"
   frameborder="0"
   allowfullscreen>
</iframe>

<a href="https://github.com/junegunn/fzf" target="_blank" rel="noopener noreferrer">
View source on GitHub ↗
</a>

---

### TMUX

`tmux` is an application that helps you create MULTIPLE terminal session inside it. It's honestly THE most important tool that I have learnt about in the pas 5 years. Instead of telling you about it, let me show you my workflow which consists:
1. Session #1 - Local
   1. Project Dir
2. Session #2 - Testing Servers
   1. Testing Server #1 - Project Dir
   2. Testing Server #1 - Project Dir
3. Session #3 - Staging Servers
   1. Staging Server #1 - Project Dir
   2. Staging Server #2 - Project Dir
4. Session #4 - Production Servers
   1. Production Server #1 - Project Dir
   2. Production Server #2 - Project Dir

Focus on the left AND right side bottom corner of the screen. That's the tmux status line. I won't even need to use the mouse to move around all these servers. Take a look. It's a long one.

<iframe
   src="https://www.youtube.com/embed/iPDIZ-EkLhA"
   style="width:100%;aspect-ratio:16/9;"
   frameborder="0"
   allowfullscreen>
</iframe>

Obviously, my tmux is customized which is why it looks nicer AND it's why I can move about so quickly. I'm using the key combinations that work for me. You can find my tmux configuration <a href="https://github.com/AaySah92/config_dotfiles" target="_blank" rel="noopener noreferrer">here ↗</a>.

<a href="https://github.com/tmux/tmux" target="_blank" rel="noopener noreferrer">
View source on GitHub ↗
</a>

---

The above list isn't exhaustive, but I wanted to show the more important ones here. Setting them up in different machines can be tricky especially if they're running completely different distributions - Debian, Arch, RHEL, etc. I'll dive into this in the next post... 🧑🏻‍💻