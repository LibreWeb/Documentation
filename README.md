# LibreWeb Documentation

The [LibreWeb Documentation](https://docs.libreweb.org) site.

## Development

Requirements:

- Hugo v0.8 or higher

Install the [latest Hugo release from GitHub](https://github.com/gohugoio/hugo/releases).

### Starting server

Start the website locally via:

```sh
hugo serve
```

By default the URL should be: [http://localhost:1313/](http://localhost:1313/).

### Changing content

The content is stored in the [content sub-directory](./content), it's using [Markdown syntax](https://www.markdownguide.org/basic-syntax/) for creating the content.

You can create new pages or change existing pages by editing the `.md` files.

We are using Hugo's markdown syntax extensions like `title`, `weight` and `description` meta-data at the top of each `.md` file. As well as a sub-folder structure.

### Git WoW

First fork this project in GitLab under your own account. This will allow you push your changes to `master` or a new branches (creating separate branch is preferred).

When you forked this project, don't forget to add the upstream git repository to your local fork/clone. Allowing you to keep in sync with the upstream remote. Via:

```sh
git clone git@gitlab.melroy.org:<your_username>/docs-website.git # Change the URL to <your_username> link of your Fork (see GitLab)
cd docs-website
git remote add upstream https://gitlab.melroy.org/libreweb/docs-website.git
git checkout master # Check-out your local master branch
git pull upstream master # Which fetches and merges the changes from upstream into your local branch
git push
```

When you already made changes in your branch, be sure to: `git add -A && git commit -am "new message"` them first before executing a `git pull upstream master`.

The last step is creating a [new merge request](https://gitlab.melroy.org/libreweb/docs-website/-/merge_requests) in GitLab. Select your fork and branch as the source, and `libreweb/docs-website` with the `master` branch as the target.

### Hugo Documentation

See the official [Hugo Getting started](https://gohugo.io/getting-started/).
