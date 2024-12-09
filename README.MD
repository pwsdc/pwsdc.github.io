# PWSDC Website

Used by the club to display meeting notes and other information.

## How the Page Works

The page is built using Hugo, a static website generator, found [here](https://gohugo.io/). The theme is PaperMod for Hugo, found [here](https://github.com/adityatelange/hugo-PaperMod). Finally, the page is deployed on GitHub Pages.

## Installing Hugo

Access to Hugo is needed to serve the site locally in order to make changes.

One method to install Hugo is via chocolatey [here](https://chocolatey.org/). Once chocolatey is installed, run:

`choco install hugo-extended`

Other installation instructions can be found [here](https://gohugo.io/installation/).

## Serving the Site Locally

To serve the site locally, clone this repo. Then, run the command:

`hugo server -D`

NOTE: This command will not rebuild the site locally on every change. If that is needed, run: 

`hugo server -D --disableFastRender`

## Add a Post

To add a post, run the command:

`hugo new posts/a-post-name.md`

This will create a new markdown file in content/posts called a-post-name.md. Other names and directories can also be chosen.

The newly generated file will contain yaml front matter. It is recommended to make changes to this section. Make sure the title is correct, and add a summary and tags section. Also remember to change "draft" to false so the page will be shown on the production site. Only change the date if you know what you're doing, as invalid dates may cause the page not to show. Here is an example front matter section:

```
+++
title = 'Test'
date = 2024-02-20T14:51:07-05:00
draft = false
summary = 'put a summary of the content here!'
tags = ['example', 'tags', 'here']
+++
```

Content for the file will go under the yaml front matter. It should follow markdown syntax.

## Shortcodes

- Superscript: see `layouts/shortcodes/super.html`
- Subscript: see `layouts/shortcodes/sub.html`

## Making Changes to the Site

GitHub Actions has been set up to build and deploy the site on the main repo. Simply push your changes, make a pull request, then when its merged the changes will be shown in a short time.

## Maintaining the Site

It is recommended to check these every so often. Make sure to test the site locally before deploying! 

PaperMod can be updated by downloading the latest source [here](https://github.com/adityatelange/hugo-PaperMod/archive/refs/heads/master.zip) and extracting the files within `hugo-PaperMod-master` to `themes/PaperMod`.

`.github/workflows/gh-pages.yml` is for GitHub Actions and is from PaperMod, the source is at `themes/PaperMod/.github/workflows/gh-pages.yml`. To update it, you will need to compare the changes manually. Do not overwrite the file directly as there are some custom changes (for example the source version has an exampleSite branch which our site doesn't).

Hugo can be updated by changing the version number in `.github/workflows/gh-pages.yml`.

`hugo.yaml` contains configuration information for the page (such as tabs in the header). More information can be found in PaperMod's documentation [here](https://github.com/adityatelange/hugo-PaperMod/wiki).
