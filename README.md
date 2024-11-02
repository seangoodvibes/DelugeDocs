# About this site

This is a static site built using the `MkDocs` platform with the theme `Material for MkDocs` which expands upon MkDocs functionality to allow for even more robust and customiable documentation website building.

- Info on MkDocs here: https://www.mkdocs.org
- Info on Material for MkDocs here: https://squidfunk.github.io/mkdocs-material

## Documentation

#### Markdown

From a documentation perspective, documentation is written in Markdown and is converted into Html automatically by the MkDocs build tool. Thus, users writing documentation do not need to worry about editing Html.

#### Editing

Each documentation page will have an Edit button so that you can easily edit the Markdown documentation. It will bring you to the Github repo where you can edit the documentation markdown file, preview your changes, and commit them to the repo.

#### Navigation

The navigation for the website (e.g. the tabs at the top, the order and hierarchy of pages in the navigation sidebar) is configured in `mkdocs.yml`

## Rebuilding the Website

After commits are made to this repo, a GitHub action will run that will re-build the website. Once this is done, the website will refresh with the changes.

# How to setup a dev environment to contribute to building this website

Follow the instructions here to install Python, Pip, and MkDocs: https://www.mkdocs.org/user-guide/installation/

You'll also want to install Material for MkDocs as instructed here: https://squidfunk.github.io/mkdocs-material/getting-started/

After you've installed the above, you can clone the repo. 

In your dev environment, use the following terminal commands:

To build the site (do this before committing any changes to the repo):
- mkdocs build

To setup a local web server that refreshes each time you save changes locally:
- mkdocs serve
