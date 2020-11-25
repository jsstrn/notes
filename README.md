# Notes

Jesstern's notes

## Development

Run the server locally and head to http://localhost:1313/ 

```bash
hugo serve
```

If you want to also include draft posts

```bash
hugo serve -D
```

## Add new content

All content is located in the `content` directory. To create a new post in `content/notes`, run 

```bash
hugo new notes/my-first-note.md
```

This will add "My first note" as the tile in the front matter of your post. To change what gets generated in the front matter, refer to documentation on [archetypes](https://gohugo.io/content-management/archetypes/#readout).

## Deploy to production

Build the project into the `public` directory

```bash
hugo
```

Then commit and push to [deploy your site to GitHub Pages](https://gohugo.io/hosting-and-deployment/hosting-on-github/#deployment-of-project-pages-from-docs-folder-on-main-branch).

## Getting help

To get help with any of the commands from the `hugo` cli tool.

```bash
hugo <command> --help
```

Otherwise, read their [documentation](https://gohugo.io/documentation/).

## Installing a theme

Select a [Hugo theme](https://themes.gohugo.io/) and run the following command

```bash
git submodule add <git-repo-url> themes/<theme-name>
```

Then go to `config.toml` and update the theme name

```toml
theme = "theme-name"
```
