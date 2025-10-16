## Introduction
This website details the methods, code, and datasets that the Risk group at Woodwell Climate Research Center uses to produce its research and work. The website is based on the [`material`](https://github.com/squidfunk/mkdocs-material) MkDocs theme. 


## File structure
- **Pages**: Each webpage is a markdown file can be found in `docs/`. The homepage is `index.md` and every other page is in `risks/`, `tools/`, or `methods/`.
- **Images**: These are kept in `/assets/images/` and subdirectories.
- **Navigation**: You can edit navigation links in `mkdocks.yml`.


## Contributing
If you are a member of the organization, you can easily contribute. To do so, you should clone this repository onto your local machine and make any edits / additions there. You can then add, commit and push your changes. Once GitHub receives your pushed changed, it will automatically rebuild and deploy the website.

To view local changes before pushing them to this repository, you can run a local server and open it in your browser. To set this up, first install the conda environment in `environment.yml` and activate it. If everything is working, you can then use this command to see a live version of the site as you make changes:
```
mkdocs serve
```

### Editing or adding webpages
To edit an existing webpage, just edit its corresponding markdown file in `risks/`, `tools/`, or `methods/`. To add a new webpage, simply copy another page's Markdown making sure to include the following lines at the top:
```
---
template: main.html

hide:
  - toc
  - path
---

```


## Acknowledgements
This repository contains code from the `material` MkDocs theme. Copyright (c) 2016-2025 Martin Donath, distributed under a MIT License.