# Writing Python with Neovim

Track: Talks
Category: ??

## Description

Neovim is a lightweight, extensible, console-based editor that works well for writing Python (and many other languages). In this talk, we will explore if Neovim is a good fit for you, and consider options for configuring it well for Python development. Topics will include linters, formatters, syntax highlighting, tab-completion, and language servers. Discussion will primarily focus around sample configuration files that can be later adapted.

## Outline

Introduction (1 minute)

Lightning tutorial on Vim/Neovim (10 minutes)
- Two modes
- Starting and quitting
- Commonly used keybindings
- Cheatsheet/documentation suggestions
- Plugins

Simplified Python configuration (3 minutes)
- Sample vimrc that works with Vim or Neovim
- No plugins required
- Simplified features

Modest Neovim config with language servers and treesitter (5 minutes)
- pyright
- null-ls + black
- treesitter for syntax highlighting

Alternate Neovim config with python-lsp-server (3 minutes)
- Configurable linting tools
- Configurable formatting tools

Other tools to consider (2 minutes)
- mason for installation of language servers, etc.
- graphical frontends such as neovide, fvim, goneovim
- jedi-language-server
- anakin-language-server
- Not into language servers? Consider Jedi-vim and Ale

Discussion (5 minutes)

## Past experience

Currently a software engineer using SQL to convert data between systems, I have been a middle and high school teacher, web developer, IT director, data wrangler, and always a hobbyist developer. I feel comfortable in front of people. I started using Vim 20 years ago, and never :q

I just presented at OLF (Ohio LinuxFest) on December 2, 2022, on using Python to manage Linux systems. Slides are available at olf22.bowmanjd.com and the video can be viewed on Youtube at https://youtu.be/DjOgRbHnvwU?t=465 (should start around 7 minutes, 45 seconds in).

A slide deck for a 2019 talk I gave at a local tech conference, introducing Python to IT professionals: bowmanjd.github.io/ttl/python-data/#1

linkedin.com/in/jonathan-d-bowman/
twitter.com/jdbowman
Various blog articles at dev.to/bowmanjd
