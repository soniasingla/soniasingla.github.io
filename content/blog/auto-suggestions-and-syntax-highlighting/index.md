---
title: How to customize Oh My Zsh with Auto-Suggestions and Syntax Highlighting?
date: "2020-10-06"
description: "As a developer, we spend a lot of time working on the terminal and having personalized shell makes the working environment perfect, decreases frustration and also, increases productivity."
---

![](./code.png)
<center><sub><sup>[Img src: https://undraw.co/illustrations]</sup></sub></center><br>

As a developer, we spend a lot of time working on the terminal and having personalized shell makes the working environment perfect, decreases frustration and also, increases productivity.

In this blog, we will discuss how to quickly install plugins `Auto-Suggestions` and `Syntax Highlighting` in the `oh-my-zsh` theme.

## Install Oh-My-Zsh using Curl:

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
<br>

**NOTE: `ZSH` and `OhMyZsh` both are different.**

Let's take a look how to install plugins, and configure `Zsh`:

## Install zsh-autosuggestions by running:

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

## Install zsh-syntax-highlighting by running:

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
```
<br>

Now, open `.zshrc` file with your favourite editor:

```bash
nano ~/.zshrc
```
<br>

And simply add `zsh-autosuggestions` & `zsh-syntax-highlighting` to `plugins()` section, it will do the magic for you:

```bash
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
```

<br>

Reopen terminal to reconfigure the settings and Voila! 🎉