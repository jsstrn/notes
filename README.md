# Notes

Jesstern's notes

## Getting started

First clone this repository

```bash
git clone git@github.com:jsstrn/notes.git
```

Then add the Git submodule and update it

```bash
git submodule init
git submodule update
```

Alternatively, you can run it all as one command

```bash
git clone --recurse-submodules git@github.com:jsstrn/notes.git
```

## Installation

First, install Hugo

```bash
brew install hugo
```

Check that Hugo was installed correctly

```bash
hugo version
```

## Development

Clone the repository

```bash
git clone git@github.com:jsstrn/notes.git
```

Update the submodule

```bash
git submodule init
git submodule update
```

Run the server locally and head to [http://localhost:1313](http://localhost:1313/notes)

```bash
npm start
```

Which runs this command

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
npm run new
```

Which runs this command

```bash
hugo new notes/my-first-note.md
```

This will add "My first note" as the tile in the front matter of your post. To change what gets generated in the front matter, refer to documentation on [archetypes](https://gohugo.io/content-management/archetypes/#readout).

The naming convention for files is `<topic>-<title>.md` (e.g. ruby-install.md)

## Publish

To publish, simply run

```bash
npm run publish
```

This runs the publish script

```bash
./publish
```

Build the project into the `docs` directory (or whichever directory is designated in `publishDir` in `config.toml`)

```bash
hugo
```

Then commit and push to [deploy your site to GitHub Pages](https://gohugo.io/hosting-and-deployment/hosting-on-github/#deployment-of-project-pages-from-docs-folder-on-main-branch).

## Installing a theme

Select a [Hugo theme](https://themes.gohugo.io/) and run the following command

```bash
git submodule add <git-repo-url> themes/<theme-name>
```

Then go to `config.toml` and update the theme name

```toml
theme = "theme-name"
```

## Customizing a theme

To customize a theme, we copy the files we want to edit into our own root folder (keeping the same folder structure). We do not edit the files directly in the theme.

## Getting help

To get help with any of the commands from the `hugo` cli tool.

```bash
hugo <command> --help
```

Otherwise, read their [documentation](https://gohugo.io/documentation/).
