📘 Hugo Basics Guide

Hugo is a fast, open-source static site generator written in Go. It’s commonly used for blogs, documentation sites, and portfolios.

📦 Installation
On Linux
sudo apt install hugo        # Debian/Ubuntu
sudo pacman -S hugo         # Arch
sudo dnf install hugo       # Fedora
On macOS
brew install hugo
On Windows

Download from: https://gohugo.io/getting-started/installing/

Check installation:

hugo version
🚀 Create a New Site
hugo new site mysite
cd mysite
🎨 Add a Theme

Browse themes: https://themes.gohugo.io/

Example using Git:

git init
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke themes/ananke

Enable the theme in hugo.toml (or config.toml):

theme = "ananke"
✍️ Create Content

Create a new post:

hugo new posts/my-first-post.md

Edit the file in content/posts/my-first-post.md:

---
title: "My First Post"
date: 2026-01-29
draft: false
---


Hello, this is my first post using Hugo!
👀 Run Development Server
hugo server

Visit: http://localhost:1313

To include drafts:

hugo server -D
🏗️ Build the Site
hugo

This generates static files in the public/ folder. You can upload this folder to any web hosting service.

📂 Project Structure
mysite/
├── archetypes/
├── content/
├── layouts/
├── public/
├── static/
├── themes/
└── hugo.toml

content/ → Your posts and pages

static/ → Images, CSS, JS

themes/ → Theme files

public/ → Final generated site

⚙️ Configuration Example (hugo.toml)
baseURL = "https://example.com/"
languageCode = "en-us"
title = "My Hugo Site"
theme = "ananke"
🧭 Useful Commands
Command	Description
hugo new site <name>	Create a new site
hugo new <path>	Create new content
hugo server	Start local server
hugo	Build the site
📚 Resources

Official Docs: https://gohugo.io/documentation/

Themes: https://themes.gohugo.io/

Community: https://discourse.gohugo.io/

If you want, I can also generate:

A Hugo blog template

A documentation site setup

A GitHub Pages deployment guide
