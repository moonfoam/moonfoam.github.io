---
title: Hexo内置标签的使用
comments: true
date: 2017-06-22 11:02:07
updated: 2017-06-22 11:02:07
tags: Hexo
categories: Blog
description: 「标签」(Tag Plugin) 是 Hexo 提供的一种快速生成特定内容的方式。 例如，在标准 Markdown 语法中，我们无法指定图片的大小，无法指定代码的高亮语言。这种情景，我们即可使用标签来解决。
---

# 引言
为了自定义[Hexo](https://hexo.io)的[NexT](http://theme-next.iissnan.com)主题，仔细研读了[NexT](http://theme-next.iissnan.com)的官方文档，才发现错过了**Tag Plugin**那么强大的功能。[NexT内置标签部分](http://theme-next.iissnan.com/tag-plugins.html)讲的相对简练，[Hexo内置标签部分](https://hexo.io/docs/tag-plugins.html#Block-Quote)则更加全。

# 标签使用

标签的使用主要分两种方式：
- HTML方式: 将标签以属性方式添加，即`class=\"标签\"`
- 标签方式: 使用`标签`或者简写进行使用

## Block Quete 块引用

> 完美地添加引用到文章，同时附带作者、来源、标题信息等附加属性

**简写**：quote

**使用**：
```
{% blockquote [author[, source]] [link] [source_link_title] %}
content
{% endblockquote %}
```
### 示例

#### 纯块引用

```
{% blockquote %}
如果我会发光，就不必害怕黑暗。如果我自己是那么美好，那么一切恐惧就可以烟消云散。于是我开始存下了一点希望。
{% endblockquote %}
```
{% blockquote %}
如果我会发光，就不必害怕黑暗。如果我自己是那么美好，那么一切恐惧就可以烟消云散。于是我开始存下了一点希望。
{% endblockquote %}

#### 引自书中
```
{% blockquote 卡森·麦卡勒斯, 《心是孤独的猎手》 %}
我去过很多地方，但我只遇到过很少的我们。
{% endblockquote %}
```
{% blockquote 卡森·麦卡勒斯, 《心是孤独的猎手》 %}
我去过很多地方，但我只遇到过很少的我们。
{% endblockquote %}

#### 引自书中
```
{% blockquote 卡森·麦卡勒斯, 《心是孤独的猎手》 %}
我去过很多地方，但我只遇到过很少的我们。
{% endblockquote %}
```
{% blockquote 卡森·麦卡勒斯, 《心是孤独的猎手》 %}
我去过很多地方，但我只遇到过很少的我们。
{% endblockquote %}

#### 引自博客
```
{% blockquote @昂翌 http://music.163.com/#/song?id=32628933 %}
最怕你一生碌碌无为，还说平凡难能可贵。
{% endblockquote %}
```
{% blockquote @昂翌 http://music.163.com/#/song?id=32628933 %}
最怕你一生碌碌无为，还说平凡难能可贵。
{% endblockquote %}

#### 引自网络文章
```
{% blockquote Seth Godin http://sethgodin.typepad.com/seths_blog/2009/07/welcome-to-island-marketing.html Welcome to Island Marketing %}
Every interaction is both precious and an opportunity to delight.
{% endblockquote %}
```
{% blockquote Seth Godin http://sethgodin.typepad.com/seths_blog/2009/07/welcome-to-island-marketing.html Welcome to Island Marketing %}
Every interaction is both precious and an opportunity to delight.
{% endblockquote %}

<!-- ### 居中引用 (Require NexT 0.4.5)

**简写**：cq

```
{% centerquote %}
Something
{% endcenterquote %}
```

{% centerquote %}
人的一切痛苦，本质上都是对自己的无能的愤怒。<br/><br/>**王小波**
{% endcenterquote %} -->

## Code Block 代码块

> 方便地添加代码片段到文章

**简写**：quote

```
{% blockquote [author[, source]] [link] [source_link_title] %}
content
{% endblockquote %}
```
### 示例
#### 纯块引用
