---
title: Quick Hexo Page Building
date: 2023-11-03 14:14:59
updated: 2023-11-03 14:14:59
tags: hexo
categories:
- web
layout: post
comment: true
cover: https://blog.getform.io/content/images/2019/10/hexo-cover-01-800x450.png
---

## Build A GitHub Page Repository

1. The repository should name after $username.github.io$.
2. In repository setting, open *page* tab, and make sure the static web is built from branch *main* or what ever you want.
3. Start web programming.

<!-- more -->

## Init Hexo Project

1. Prepare two tools: node.js and git

2. install follow guide below:

   ```bash
   $ npm install -g hexo-cli
   ```

3. Create a new folder, and

   ```bash
   $ hexo init <new folder>
   $ cd <new folder>
   $ npm install
   # remember to replace <new folder>
   ```

4. Connect the folder to your github repository.

**Some file or folder noticeable:** *_config.yml* for page config, *package.json* for app info, *scaffolds* is template of articles, and *theme* is … theme.



## Configuration

Configuration to your page will be at **_config.yml**. Most of the part is very easy, just like json or dictionary in python. Here I list some key-value pairs that need to be noticed(just for example. You should modify them yourself.).

| key                    | value                                                        |
| ---------------------- | ------------------------------------------------------------ |
| `language`             | zh-CN/EN…                                                    |
| `timezone`             | Asia/Shanghai…                                               |
| `permalink`            | permanent link format of article, In default it will be like  2013/07/14/hello-world/, I prefer :category/:title/. And you can play some trick here to make a multi-language page. |
| `external_link`        | Open new tab in link                                         |
| `external_link.enable` | Open new tab in link                                         |

Customize your directory in *directory* part.



## Common Command

1. Init Hexo project

   ```bash
   hexo init [folder]
   ```

   

2. New article

   ```bash
   hexo new [--path/--replace/--slug] <title>
   ```

   

3. Generate

   ```bash
   hexo generate [--deploy/--bail]
   ```

   

4. Publish draft

   ```bash
   hexo public [layout] <title>
   ```

   

5. Launch server

   ```bash
   hexo server
   ```

   visit [(http://localhost:4000/](http://localhost:4000/)

6. Deploy

   ```bash
   hexo deploy
   ```




## Theme

Choose a beautiful and convenient theme is pretty important.

visit [theme](https://hexo.io/themes/) to pick one you like, every theme has unique installation in its own page.



## Deploy to Github

Want to have a free static page can be visit? The step can’t be ignored.

1. Build a repository in Github named after “[your username].github.io”.

2. Setting -> Pages -> Action: Github Action.

3. Create new file “.github/workflows/pages.yml” in your hexo project.

4. Copy contents below to the file, change all “20” to your node version.

   ```yaml
   name: Pages
   
   on:
     push:
       branches:
         - main # default branch
   
   jobs:
     build:
       runs-on: ubuntu-latest
       steps:
         - uses: actions/checkout@v3
           with:
             token: ${{ secrets.GITHUB_TOKEN }}
             # If your repository depends on submodule, please see: https://github.com/actions/checkout
             submodules: recursive
         - name: Use Node.js 20.x
           uses: actions/setup-node@v2
           with:
             node-version: '20'
         - name: Cache NPM dependencies
           uses: actions/cache@v2
           with:
             path: node_modules
             key: ${{ runner.OS }}-npm-cache
             restore-keys: |
               ${{ runner.OS }}-npm-cache
         - name: Install Dependencies
           run: npm install
         - name: Build
           run: npm run build
         - name: Upload Pages artifact
           uses: actions/upload-pages-artifact@v2
           with:
             path: ./public
     deploy:
       needs: build
       permissions:
         pages: write
         id-token: write
       environment:
         name: github-pages
         url: ${{ steps.deployment.outputs.page_url }}
       runs-on: ubuntu-latest
       steps:
         - name: Deploy to GitHub Pages
           id: deployment
           uses: actions/deploy-pages@v2
   ```

   

## Enjoy your hexo journey!