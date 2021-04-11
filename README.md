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

### Hugo Documentation

See the official [Hugo Getting started](https://gohugo.io/getting-started/).
