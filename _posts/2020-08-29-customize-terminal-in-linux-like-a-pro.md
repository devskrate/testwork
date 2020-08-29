---
date: 2020-08-29 09:26:40
layout: post
title: How to customize your terminal like a developer and for good feel
subtitle: "Turn your Terminal like a pro"
description: >-
  Generally the terminals that we get from the different linux distributions are good but the only thing is, they are not good looking.
image: >-
  https://devskrate.github.io/assets/blog-banners/bbk-tech.jpg
optimized_image: >-
  https://devskrate.github.io/assets/blog-banners/optimized/bbk-tech.webp
category: [dev]
tags: [terminal, linux, pro, debian, terminator]
author: puneeth
is_generated: true
---

Generally the terminals that we get from the different linux distributions are good but the only thing is, they are not good looking. Actually they are nice but lack some details that most of them like to have. 

Here we will show you how to install most popular themes for your terminal..

Some of the popular themes are 
+ Ohmyzsh
+ Ohmyfish
+ FancyBashPrompt and some others..

Let's see the installation of the Ohmyzsh. Before actually using it in your default terminal try to apply on another terminal.

+ I use Gnome-Terminal as my default shell, to test this I downloaded **Terminator**. If you want to test it in terminator, then install terminator by `sudo apt install terinator`
+ Now check if you have `zsh` installed in your system. Type `zsh --version`. If you get a version number as response, then you have already installed it!
+ Now we need to install the Ohmyzsh theme.. For that install the script by using any of the following method..
    - **Via curl**
    ```bash
    sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    ```
    - **Via wget**
    ```bash
    sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    ```
    - **Via fetch**
    ```bash
    sh -c "$(fetch -o - https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    ```
Boom, you have just installed the theme! But you need more to do for customizing it..

+ Go to this link [https://github.com/ohmyzsh/ohmyzsh/wiki/Themes](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes) and note down the name of the theme you like.

+ Now just type `nano ~/.zshrc` in the terminal. We are using nano editor for editing the `.zshrc` file. You can also use your own one's but recommended is nano.

+ You can see a line `ZSH_THEME="robbyrussell"`. Now in the place of `robbyrussell` or any other insert your theme name that you liked in the above step.

+ **Note** :
Some of the themes need [PowerLine Fonts](https://github.com/powerline/fonts). You can directly install it if you are in a Debian or Ubuntu based systems by `sudo apt-get install fonts-powerline`. 

I use `agnoster` theme and it looks like this..

<div class="slide-show">

<a href="https://devskrate.github.io/assets/images/dev/terminal/customize-terminal.jpg" data-lightbox="image-1" data-title=""><img width="85%" src="https://devskrate.github.io/assets/images/dev/terminal/customize-terminal.jpg"></a>

</div>

**Links for devs and interested**:

- Ohmyzsh : [https://github.com/ohmyzsh/ohmyzsh](https://github.com/ohmyzsh/ohmyzsh)
- PowerLineFonts : [https://github.com/powerline/fonts](https://github.com/powerline/fonts)
- Ohmyfish : [https://github.com/oh-my-fish/oh-my-fish](https://github.com/oh-my-fish/oh-my-fish)