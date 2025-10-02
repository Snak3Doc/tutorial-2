---
layout: ../../layouts/MarkdownPostLayout.astro
title: "Dynamic Dispay of New Blog Posts"
pubDate: 03/09/2025
description: "Learning how to use `meta.glob()`"
author: "SnakeDoc"
image:
    url: "https://docs.astro.build/assets/rays.webp"
    alt: "The Astro logo on a dark background with rainbow rays."
tags: ["astro", "blogging", "learning astro"]
---

## The Problem

As more posts are added to the blog, it becomes annoying and repetative to add a new list item for every new blog post thats created.

## The Solution

To solve this we created a varaible `allPosts` in `blog.astro`, the values for this this variable come from using `import.meta.glob('./posts/*.md')` this looks in the posts folder using the wildcard `*` to search for any filename with the `.md` extension