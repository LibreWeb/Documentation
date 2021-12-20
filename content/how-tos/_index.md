---
title: "How-tos"
weight: 4
description : "How-tos and tutorial for LibreWeb Browser to help you"
---

No matter what you are looking for, we have a tutorial and how-tos to help you.

## Getting started - Installing LibreWeb Browser

Visit the [releases page](https://gitlab.melroy.org/libreweb/browser/-/releases "External link"). Download the correct package for your Linux distribution.

### Advanced users - Verifying GPG signature of LibreWeb Browser

Verifying the LibreWeb Browser via GNU Privacy Guard (GPG), used to verify the authenticity of the binary.

{{%expand "Show How-to verify LibreWeb applications via GPG." %}}

#### Import the signing key from keyserver

Import the public key from [Melroy Antoine van den Berg](https://keys.openpgp.org/search?q=E0C7C029005B0CE6A7438BD571D11FF23454B9D7 "External link").

Type this in a terminal (or copy):

```sh
gpg --keyserver keys.openpgp.org --recv-keys E0C7C029005B0CE6A7438BD571D11FF23454B9D7
```

#### Verify the fingersprints

```sh
gpg --fingerprint E0C7C029005B0CE6A7438BD571D11FF23454B9D7
```

You should see:

```sh
pub   rsa3072 2021-04-06 [SC]
      E0C7 C029 005B 0CE6 A743  8BD5 71D1 1FF2 3454 B9D7
uid           [ unknown] Melroy Antoine van den Berg <melroy@melroy.org>
sub   rsa3072 2021-04-06 [E]
```

#### Download the Browser and the signature file (asc)

[Download the LibreWeb Browser](https://gitlab.melroy.org/libreweb/browser/-/releases "External link") as well as the corresponding signature file (.asc).

#### Verify signature of the downloaded file

As an example we will take the Debian/Ubuntu package:

```sh
gpg --verify libreweb-browser-v0.6.0.deb.asc libreweb-browser-v0.6.0.deb
```

The output should say “Good signature from "Melroy Antoine van den Berg <melroy@melroy.org>"”:

```sh
gpg: Signature made Wed 07 Apr 2021 12:51:23 AM CEST
gpg:                using RSA key E0C7C029005B0CE6A7438BD571D11FF23454B9D7
gpg: Good signature from "Melroy Antoine van den Berg <melroy@melroy.org>" [unknown]
gpg: WARNING: This key is not certified with a trusted signature!
gpg: There is no indication that the signature belongs to the owner.
```

Notice that there is a warning because you haven't assigned a trust index to this person (which can be ignored).

```sh
gpg: WARNING: This key is not certified with a trusted signature!
gpg: There is no indication that the signature belongs to the owner.
```

This means that GnuPG verified that the key made that signature, but it's up to you to decide if that key really belongs to the developer. The best method is to meet the developer in person and exchange key fingerprints.

{{% /expand%}}

## How to deploy my site/blog?

LibreWeb is using the **[markdown format](https://www.markdownguide.org/basic-syntax/)** as the document source-code, instead of HTML code.   
LibreWeb will load, parse and display the markdown files, directly within the LibreWeb Browser, visually.

If you are already using static site generators like Hugo or Jekyll to generate your site, you are already future-proof for LibreWeb (the difference is you don't need the build step).

LibreWeb has a built-in markdown editor that allows you to easily write your own site without the need for technical skills. Moreover, LibreWeb will soon have additional features that will allow you to deploy fully functional sites and rich content on IPFS - like you can with Hugo and Jekyll - *without* the need to know or write any HTML.

## How to browse content?

Currently, you can visit pages in the address bar at the top of the browser. 

*WIP:* Once we have a decentralized nameserver solution in place (IPNS or alike). You will be able to visit pages using a human readable domain names.

## How to find other websites?

*WIP:* We way want to implement a decentralized store, where you can store your metadata about your website. So no spiker/webcrawler or centralized solution should be needed to search the decentralized web.

In the meanwhile, you need to know the content hash (also known as `CID`) of the file/site to you want to visit.

## How to contribute to LibreWeb Documentation?

In order to contribute to LibreWeb Docs (this site), you should be have some basic knowledge about:

1. [Git](#git) - See below
2. Markdown syntax - [Take a look at the markdown basics](https://www.markdownguide.org/basic-syntax/ "External link")

After this, you should be able to edit a page (notice the: "<i class="fas fa-code-branch"></i> Edit this page" link in the right-top corner).  
Fork the git project in GitLab. Edit directly in GitLab. *Or* add your SSH public key to your GitLab profile and execute: `git clone git@gitlab.melroy.org:your_username/docs-website.git` (change `your_username`) to fork project locally on your computer. Next, go to the project folder: `cd docs-website`.

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

The last step is creating [creating a merge Request](https://gitlab.melroy.org/libreweb/docs-website/-/merge_requests "External link") in GitLab. Select your fork and branch as the source and select `libreweb/docs-website` with the `master` branch as target.

{{% notice info %}}
Instead of making your changes directly on your `master` branch, it's advised that you create small incremental changes via seperate branches.  
Create a new branch via: `git checkout -b my_new_branch_name`.
{{% /notice %}}

### Git

I attached a well written book about Git. As well as a handy Git cheat sheet, which you can download below:

{{%attachments title="Related files" style="blue" pattern=".*(pdf)" /%}}
