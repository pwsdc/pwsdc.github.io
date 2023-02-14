---
title: "Developing the Website"
date: 2023-02-14T12:53:14-05:00
draft: false
summary: How to develop and deploy the website.
---

The website is built with Hugo and deployed on GitHub pages.

## Install Hugo

First, install Go.

Then install hugo. (With chololatey on windows.)

`choco install hugo-extended`

Use hugo to serve the site on a local server for development.

`hugo server -D`

## Add a post.

`hugo new posts/a-post-name.md`

This will create a new markdown file in content/posts.

Add markdown content under the yaml front matter.

The post will appear in the website posts.

## Build

`hugo` will build to `public`.

Github Pages should be configured to deploy from /public.
