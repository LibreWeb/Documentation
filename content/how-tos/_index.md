---
title: "How-tos"
weight: 4
description : "How-tos and tutorial for LibreWeb Browser to help you"
---

No matter what you are looking for, we have a tutorial and how-tos to help you.

## Getting started - Installing LibreWeb Browser

Visit the [releases page](https://gitlab.melroy.org/libreweb/browser/-/releases "External link"). Download the correct package for your Linux distribution.

## How to deploy my site/blog?

LibreWeb is using markdown files as source instead of HTML.

You should be future-proof for LibreWeb if you currently use static site generators like Hugo or Jekyll to generate your site.

LibreWeb has a built-in markdown editor that allows you to easily write your own site without the need for technical skills. Moreover, LibreWeb will soon have additional features that will allow you to deploy fully functional sites and rich content on IPFS - like you can with Hugo and Jekyll - *without* the need to know or write any HTML.

## How to browse content?

TODO

## How to find other websites?

TODO

## How to contribute to LibreWeb Documentation?

In order to contribute to LibreWeb Docs (this site), you should be have some basic knowledge about:

1. [Git](#git) - See below
2. Markdown syntax - [Take a look at the markdown basics](https://www.markdownguide.org/basic-syntax/ "External link")

After this, you should be able to edit a page (notice the: "<i class="fas fa-code-branch"></i> Edit this page" link in the right-top corner).  
Fork the git project in GitLab. Edit directly in GitLab. *Or* add your SSH public key to your GitLab profile and execute: `git clone git@gitlab.melroy.org:your_username/docs-website.git` (change `your_username`) to fork project locally on your computer. Go to your git project folder: `cd docs-website`.

You should now be able to make changes in your fork you just cloned on your computer.  
The git development cycle is as follows:

```sh
git remote add upstream https://gitlab.melroy.org/libreweb/docs-website.git # Add the original repository as upstream remote in git
git checkout master # Be sure we're on the master branch
git commit -am "My changes" # If applicable, commit your changes (execute "git add -A" before, if you also added new files)
git fetch upstream # Get the latest changes from upstream remote
git merge upstream/master master # Merge with the upstream remote into your local master branch fork
git push
```

The last step is creating [creating a Merge Request](https://gitlab.melroy.org/libreweb/browser/-/merge_requests "External link") in GitLab. Select your fork and branch as the source and select `libreweb/docs-website` with the `master` branch as target.

{{% notice info %}}
Instead of making your changes directly on your `master` branch, it's advised that you create small incremental changes via seperate branches.  
Create a new branch via: `git checkout -b my_new_branch_name`.
{{% /notice %}}

### Git

I attached a well written book about Git. As well as a handy Git cheat sheet, which you can download below:

{{%attachments title="Related files" style="blue" pattern=".*(pdf)" /%}}