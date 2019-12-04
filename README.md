# Git Repo for UNH Cyber Security Club Website

This repository holds the source files for the UNH Cyber Security Club website being developed in ENGL502.

## Setup

The website is using [Hugo](https://gohugo.io/) to make maintaining and updating the site easier.

To develop the project, install hugo and run `hugo server -D` to build a local development version of the site.

To edit the layout of the site, edit the templates in `theme/cyber/layouts/`. The file `index.html` is for the homepage. Partials are parts of websites that are repeatedly used and can be called easily using their name. `_default` contains the layout for the rest of the pages with `baseof.html` defining the base layout. The `main` section is defined in both `list.html` and `single.html`, if the page is an article it uses `single.html` otherwise it uses `list.html`

To add content to the website, add a file or folder to `content/` using the command `hugo new [path]/[filename].md`, due to a bug to add to `content/resources`  you have to use the command `hugo new content/resources/[rest_of_path]/[filename].md`.