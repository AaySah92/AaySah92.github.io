---
title: "Automating CLI Setup Across Multiple Linux Distributions"
layout: post
tags:
   - Linux
   - Linux Distributions
   - CLI
   - Automation
---

Depending on the day of the week, I work on 1-3 different Linux distributions; at a point, this number went up to 4.
- Arch - used to be on my personal laptop; I've since moved to Fedora.
- Ubuntu - a temporary Linode web server that hosted my wedding site.
- A corporate-backed distribution for work.
- Debian - on WSL2 for development on Windows (I know... I'm not proud of this).

It's important for me to the have my <a href="{% post_url 2025-12-15-cli-essentials %}" target="_blank" rel="noopener noreferrer">CLI essentials</a>
installed on every system I work on, so I can maintain the same workflow. For instance, when I use TMUX, no matter which system I'm on, CTRL+A should be the prefix key. Or when I press CTRL+R on the terminal, I want to be able to scroll through my command history.

To achieve this, one way is to manually install the required packages and download <a href="https://github.com/AaySah92/config_dotfiles" target="_blank" rel="noopener noreferrer">my configuration</a> from Github into the `~/.config` directory on each system. As an engineer, it triggers me to repeat a set of tasks _too many times_ (it's important to know when it's okay to repeat something and when it becomes a bottleneck). In an ideal world, there should be a tool/script that does all of this, regardless of which Linux distribution is installed on the system.

Basically, I am talking about automation. By far, the easiest way to automate this process would be to use shell scripting, but it does not address 3 major issues involved with installing packages across multiple Linux distributions:

1. Different package managers:
    - Arch uses `pacman`, Debian uses `apt`, Fedora uses `dnf`. When making a shell script, you would have to make sure it supports as many package managers as possible. 
    - This means more maintenance work and limitations on distributions the script can support. Not to mention how horrible the code would look with all it's configuration or worse - IF CONDITIONS. 
2. Different names of the same package across multiple package managers:
    - Some developers, for reasons I don't know, decide to name their tools differently for different package managers. For instance, Apache HTTP Server is named `apache2` on Debian but `httpd` on Fedora.
    - This means, just like before, more maintenance. You'd have to maintain multiple names of each required package per package manager.
3. Different versions of the same package installed by different distributions:
    - If the package version is not specified in the script, the default/latest version of the package would be installed on the system. But the definition of the "latest version" changes from distribution to distribution. For any given package, there's a high chance Debian would install an older version (stable) as opposed to the latest version (bleeding edge) installed by Fedora. 
    - This could even differ if you're on different version of the same distribution. For instance, Ubuntu 25.04 would install `fzf` v0.60.3 whereas Ubuntu 26.04 would v0.67.0.
    - This is the most important downside of using shell scripts. Here's why:
      - Some features may be missing in the older versions. Imagine trying to use the bash integrations of `fzf` but they don't work because you're using an older version of Ubuntu. 
      - Your configuration might start failing since it's not compatible with the older OR newer version of the package installed.
    - To avoid this issue, you'd have to specify the oldest common version across all the supported distributions. This comes ata major cost of missing latest features.

That was probably a LOT to take in... In short, automation using shell scripting isn't the best solution to the problem at hand. I'll explore another solution in the next post. But before I move on, let me clarify the exact features I need.

1. Install a list of packages across major Linux distributions.
2. Ensure same package versions are installed across all distributions.
3. Download and save the user's configuration from Github into their `~/.config` directory.
4. Easy to remove all configuration and uninstall all packages if/when required.
5. Minimal maintenance.
6. Easy to set up.
