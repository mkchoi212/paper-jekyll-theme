---
layout: post
title: "Quick Start Guide"
description: "How to setup and use the blog"
date: 2017-07-21
tags: jekyll
comments: true
---

<script async defer src="https://buttons.github.io/buttons.js"></script>

<p align="center">
  <img src="https://deadbeef.me/paper-jekyll-theme/assets/paper-cover-photo.png">
  <p align="center">
     A minimalistic Jekyll Theme
     <br>
     <br>
     <a class="no-hov" href="https://travis-ci.org/mkchoi212/paper-jekyll-theme"><img src="https://travis-ci.org/mkchoi212/paper-jekyll-theme.svg?branch=master"></a>
     <a class="no-hov" href="https://raw.githubusercontent.com/mkchoi212/paper-jekyll-theme/master/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg"></a>
     <br><br>
     <a class="github-button" href="https://github.com/mkchoi212/paper-jekyll-theme" data-size="large" data-show-count="true" aria-label="Star mkchoi212/paper-jekyll-theme on GitHub">Stars</a>
  </p>
</p>
<br>

Paper is a minimal Jekyll theme. Perfect for hosting your personal site, blog, or portfolio on GitHub or self-hosting on your own server. The styling is purposely minimalistic so that you can add your own flare to the website.

I'm currently using this theme on my [personal blog](https://www.deadbeef.me).

## Features
- Compatible with Jekyll 3.x and Github Pages
- Live local reloading for faster development
- **Responsive layout** built-in
- Supports Jekyll's built-in Sass/SCSS preprocessor
- Supports **Google Analytics**
- Supports **Disqus** for commenting
- Minimum Dependencies
- Rakefile for automation
    - `rake check`    - Check links/html files of the generated site
    - `rake clean`    - Clean up generated site
    - `rake post`     - Begin a new post in `./_posts`
    - `rake preview`  - Preview with livereload on local machine

## Usage
```
git clone https://github.com/mkchoi212/paper-jekyll-theme.git
bundle install
rake preview
```

Then, go to your favorite brower and type in the address `http://127.0.0.1:YOUR_PORT_NUM_HERE` to preview your website.

### Customization
To customize various details - title/description of the website, your SNS accout names, etc - edit the `_config.yml` file. 

### Adding posts
```
rake post title="A Title" [date="2012-02-09"] [tags=[tag1,tag2]] [category="category"]
```
This will create a markdown file in the default folder where all posts are stored in Jekyll; `_post`.

If you wish to **change the directory where posts are saved**, go to the `Rakefile` and edit the `CONFIG = { 'posts': CUSTOM_PATH_HERE }`. This will allow `rake post` to know where to save the new posts to.

The **drafts** you are working on can be saved in the `_drafts` directory. When you push your code to the server, files in this directory will NOT be included to the list o posts.

# Licnese
The MIT License (MIT)

Copyright (c) 2017 Mike JS. Choi

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
