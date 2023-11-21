---
title: Running a Hexo Project - Writing
date: 2023-11-03 15:09:43
updated: 2023-11-03 15:09:43
tags: hexo
categories: 
- 学习
- 计算机
- 工具
layout: post
comment: true
cover: https://blog.getform.io/content/images/2019/10/hexo-cover-01-800x450.png
---

hexo博客搭建后的运营工作
<!-- more -->
***Before the beginning of everything, learn syntax of markdown first please.***


## New Article

```bash
 hexo new [layout] <title>
```

layout has 3 option:

1. post: like an article.
2. draft: draft of an article, can become a page or post using `publish` command.
3. Page: new a page instead of a post.



## Configuration of an Article

Have you find the content between  `- - - ` in front of your article? Configure your article through these key-value.

| Setting      | Description                                                  | Default                                                      |
| :----------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| `layout`     | Layout                                                       | [`config.default_layout`](https://hexo.io/docs/configuration#Writing) |
| `title`      | Title                                                        | Filename (posts only)                                        |
| `date`       | Published date                                               | File created date                                            |
| `updated`    | Updated date                                                 | File updated date                                            |
| `comments`   | Enables comment feature for the post                         | `true`                                                       |
| `tags`       | Tags (Not available for pages)                               |                                                              |
| `categories` | Categories (Not available for pages)                         |                                                              |
| `permalink`  | Overrides the default permalink of the post. Permalink should end with `/` or `.html` | `null`                                                       |
| `lang`       | Set the language to override [auto-detection](https://hexo.io/docs/internationalization#Path) | Inherited from `_config.yml`                                 |

Categories Has hierarchy but tags not.

```
categories:
- [Diary, PlayStation]  # juxtapose
- [Diary, Games]
- [Life]  # Lowerlevel
```

Place where you want to show in home page part a 
```html
<!-- more -->
```


## Embed Resource

First you need to

```bash
npm i hexo-tag-embed
```

### Quoting from scriptures

```bash
{% blockquote [author[, source]] [link] [source_link_title] %}
content
{% endblockquote %}
```

## Plug in Code Block

```bash
{% codeblock [title] [lang:language] [url] [link text] [additional options] %}
code snippet
{% endcodeblock %}
```

## Youtube

```bash
{% youtube video_id [type] [cookie] %}
```

## From Other Article

```bash
{% post_path filename %}
{% post_link filename [title] [escape] %}
```

## Picture

Can be implement just easy like html

```html
<img src="" title="" alt="" class="" width="" height="">
```

## Video

```html
<iframe width="560" height="315" src="your/vedio/url/here" frameborder="0" allowfullscreen></iframe>
```

Important: remember to add an embed video url instead of url of whole page.

## Resource in Assets Folder

```bash
{% asset_path filename %}
{% asset_img [class names] slug [width] [height] [title text [alt text]] %}
{% asset_link filename [title] [escape] %}
```



## Let's start blog here!

