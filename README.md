# indic-awashedupnerd

Depolyed on ![github pages](https://github.com/TeamYayin/indic-awashedupnerd/workflows/github%20pages/badge.svg)

Current Theme [LoveIt](https://hugoloveit.com/)

[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/TeamYayin/indic-awashedupnerd)

## Creating New Posts

### Prefered

- Create a new folder in `posts` folder in `content` folder with same name as title of posts
- In name do not add space and replace it with hyphen `-` and try naming folder in english.
- create a file named `index.md` or `index.en.md` and write post contents in it following below syntax.
- for telugu version create a file with name `index.te.md` in same folder.
- for hindi `index.hi.md` or other langauges replace it respective two letter code.
- Add all related images about post in the new folder, main image to be added in `featured-image`.

### Second way

- Create a new markdown file in `content` folder with same name as title of post `post-name.md`
- In name do not add space and replace it with hyphen `-`
- write post or song or commentary by following below structure.
- For English version copy the file contents into new file named `post-name.en.md`

## New Post Structure and Metadata

Always start new post with following lines then write actual content

```yml
---
weight: 1
title: "Post title or కవిత పేరు" # the writing langauage name is good
date: 2019-03-09 # replace with current date
draft: false  # if post is still a draft then change to true
tags: ["test"] # include related tags
categories: ["test"] # include category
author: "Nidhi" # Telugu or Hindi script is good
authorLink: ""
description: "Lorem Ipsum Dolor Si Amet." # about the post in a line
timeToRead: "10" # reading time estimate

resources:
  - name: "featured-image" # post image visible in home page and in post webpage
    src: "hero-4.jpg" # file name & for now should be in same folder

lightgallery: true
hiddenFromHomePage: false # if true -- post no visible in home page

toc:
  auto: false # index
---

Content to be displayed in home page under title. Include something like a abstract or small description or type in between actual content. This content will also be visible in post webpage <!--more-->

The Actual content

```

## Creating new pages

- Create a new file with like `pagename.md` or `pagename.en.md` in `page` folder under `content`

- follow this structure

```yml
---
weight: 1
title: "page title or టైటిల్" # langauge script supported
subtitle: "sub title for page aka సబ్ టైటిల్ ఉంటే ఇక్కడ రాయండి"
date: 2019-03-06
draft: false
lightgallery: true
---

write page content in markdown here

```

## Helpful tips for writing in Hugo

- use `##` big heading like above section name or `###` or `####` for headings.

- to add new hyperlink like [google.com](https://www.google.com/) use:

```md
[google.com](https://www.google.com/)
```

- to add image use both local and from internet

```md
![Tux, the Linux mascot](/assets/images/tux.png)
![nidhi-logo](https://images.pexels.com/photos/207691/pexels-photo-207691.jpeg)
```

![nidhi-logo](https://images.pexels.com/photos/207691/pexels-photo-207691.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=457&w=640)

- to make text bold use `**bold text**` **bold text**.

- to make italic use `*cat's meow*` _cat's meow_.

- to make text bold and italic use `***cat's meow***` **_cat's meow_**.

- To create a blockquote, add a > in front of a paragraph.

`md > Dorothy followed her through many of the beautiful rooms in her castle.`

- to make list use `-` or number them

```md
- test 1
- test 2
  - test 2.1

1.  test 1
2.  test 2
3.  test 2.1
```

1. First item
2. Second item
3. Third item
   1. Indented item
   2. Indented item
4. Fourth item

- To create a horizontal rule, use three or more dashes `---` on a line by themselves and put blank lines before and after horizontal rules.

  ***

- to add figure like charts or more than images use

```go
{{< figure src="/media/spf13.jpg" title="Steve Francia" >}}
```

- to include a single tweet into your blog post, we will need is the URL of the tweet: like this tweet id

<https://twitter.com/spf13/status/877500564405444608>

```go
{{< tweet 877500564405444608 >}}
```

- to include youtube video like this song use id of the video i.e text after ?v=

<https://www.youtube.com/watch?v=8PiwQJHtN8s>

```go
{{< youtube 8PiwQJHtN8s >}}
```

## LICENSE

MIT
