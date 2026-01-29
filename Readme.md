# Hugo Basics Guide

Hugo is a fast, open-source static site generator written in Go.  
It’s commonly used for blogs, documentation sites, and portfolios.

As of early 2026, the latest version is around **v0.155** – **v0.156-dev** (check `hugo version` or the [official releases](https://github.com/gohugoio/hugo/releases) for the exact current release).

## 📦 Installation

### On Linux
```bash
sudo apt install hugo       # Debian / Ubuntu
sudo pacman -S hugo        # Arch
sudo dnf install hugo      # Fedora# Hugo Basics Guide

Hugo is a fast, open-source static site generator written in Go.  
It’s commonly used for blogs, documentation sites, and portfolios.

As of early 2026, the latest version is around **v0.155** – **v0.156-dev** (check `hugo version` or the [official releases](https://github.com/gohugoio/hugo/releases) for the exact current release).

## 📦 Installation

### On Linux
```bash
sudo apt install hugo       # Debian / Ubuntu
sudo pacman -S hugo        # Arch
sudo dnf install hugo      # Fedora
```
#### create a new site
```bash 
hugo new site mysite
cd mysite
```


#### create content
```bash
hugo new posts/my-first-post.md
```
this will reselut in blog template
---
title: "My First Post"
date: 2026-01-29
draft: false
---

Hello, this is my first post using Hugo!



for demo you can run server locally
```bash
hugo server
````

#### basic config 
```bash
baseURL      = "https://example.com/"
languageCode = "en-us"
title        = "My Hugo Site"
theme        = "ananke"

[params]
  description = "A simple blog built with Hugo"
  ```
