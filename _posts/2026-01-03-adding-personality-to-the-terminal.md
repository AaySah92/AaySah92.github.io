---
title: "Adding Personality to the Terminal"
layout: post
tags:
   - Linux
   - Terminal
   - Alacritty
   - TMUX
---

Using the terminal as-is can be a bit of a dull experience. For instance, this is how you'd interact with the CLI on a fresh Linux Mint installation. 

<iframe
src="https://www.youtube.com/embed/mEVNZoGkH8Q"
style="width:100%;aspect-ratio:16/9;"
frameborder="0"
allowfullscreen>
</iframe>

It's very basic, and it wouldn't hurt to add a little personality to it. So, let's do just that...

## Install Nerd Fonts

This is crucial for making the terminal experience better. I use these fonts in multiple tool's configurations (see below) to make sure fonts on the terminal remain uniform. It involves a couple of steps which aren't straight forward if you're new to this. 

<iframe
src="https://www.youtube.com/embed/H0Lg8UdMqHc"
style="width:100%;aspect-ratio:16/9;"
frameborder="0"
allowfullscreen>
</iframe>

## Use a better terminal emulator - Alacritty

The default terminal emulator for any distro depends on the desktop environment. 

| Desktop Environment | Default Terminal Emulator |
|---------------------|---------------------------|
| GNOME               | GNOME Terminal            |
| KDE                 | Konsole                   |
| XFCE                | Xfce Terminal             |
| LXDE / LXQt         | LXTerminal                |

They get the job done, but I prefer **Alacritty**. There are two reasons: great default settings (so I don't have to change much) and the ability to configure everything using a TOML file. The TOML file should be located in the users config directory - `~/.config/alacritty/alacritty.toml`. I have uploaded my Alacritty config file in <a href="https://github.com/AaySah92/config_dotfiles" target="_blank" rel="noopener noreferrer">my public Github repo</a> so I can access it from anywhere. Below, you can see how Alacritty looks out of the box, and later, how it looks after a few configuration changes.

<iframe
src="https://www.youtube.com/embed/RpnmRQWjnaQ"
style="width:100%;aspect-ratio:16/9;"
frameborder="0"
allowfullscreen>
</iframe>

## Customize the prompt - Oh My Posh

There are other modern, customizable prompts out there, but my favourite by far is **Oh My Posh**. It comes with a bunch of great themes, and I personally prefer Catppuccin, since it's one of those themes that's available for multiple tools such as TMUX and NeoVim.

<iframe
src="https://www.youtube.com/embed/0cJnoZ7yMtE"
style="width:100%;aspect-ratio:16/9;"
frameborder="0"
allowfullscreen>
</iframe>

You can find a list other Oh My Posh themes <a href="https://ohmyposh.dev/docs/themes" target="_blank" rel="noopener noreferrer">here</a>.

In case you're not happy with the themes that Oh My Posh offers, here are some alternatives for the bash shell:
1. <a href="https://starship.rs/" target="_blank" rel="noopener noreferrer">Starship</a>
2. <a href="https://ohmybash.nntoan.com/" target="_blank" rel="noopener noreferrer">Oh My Bash</a>
3. <a href="https://github.com/b-ryan/powerline-shell" target="_blank" rel="noopener noreferrer">Powerline</a>

## Customize TMUX

Finally, it's time for TMUX. TMUX is THE most important tool for me. It's not awful to look at but few little changes can make it look way better. It's one of those tools that has a whole ecosystem around it. It has plugin manager called <a href="https://github.com/tmux-plugins/tpm" target="_blank" rel="noopener noreferrer">TPM</a>. Once it's installed, you can start adding plugins such as a _theme_ plugin called Catppuccin. You will have to do this via the TOML configuration file. Let me show you how.

<iframe
src="https://www.youtube.com/embed/e4KhLM6a42I"
style="width:100%;aspect-ratio:16/9;"
frameborder="0"
allowfullscreen>
</iframe>

You can find a list other TMUX themes <a href="https://github.com/rothgar/awesome-tmux?tab=readme-ov-file#themes" target="_blank" rel="noopener noreferrer">here</a>.

## That's it

By following 4 simple steps, you can change the look and feel of your terminal. In the next post, I'll present the challenge you will face setting up <a href="{% post_url 2025-12-15-cli-essentials %}" target="_blank" rel="noopener noreferrer">CLI essentials</a> along with all these customizations on different Linux distributions. 