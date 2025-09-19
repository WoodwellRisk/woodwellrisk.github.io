## Introduction
This website details the methods, code, and datasets that the Risk group at Woodwell Climate Research Center uses to produce its research and work. The website is based on the [`minimal-mistakes`](https://github.com/mmistakes/minimal-mistakes) Jekyll theme. 


## File Structure
- **Pages**: Each webpage is a markdown file and these are found in `_pages/`, with the exception of `index.md` in the root directory. This file is the home page.
- **Image Files**: These are kept in `/assets/images/` and subdirectories.
- **Navigation Bar**: You can edit navigation bar in `_data/navigation.yml`.


## Contributing
If you are a member of the organization, you can easily contribute. To do so, you should clone this repository onto your local machine and make any edits / additions there. You can then add, commit and push your changes. Once GitHub receives your pushed changed, it will automatically rebuild and deploy the website.

To view local changes before pushing them to this repository, you can run a local server and open it in your browser. To set this up, follow the instructions on this [GitHub Pages explainer](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll). If everything is working, you can use this command to see a live version of the site as you make changes:
```
bundle exec jekyll serve
```

### Editing Webpages
To edit an existing webpage, just edit its corresponding markdown file in `_pages/`.

### Adding new webpages
Make a copy of `_pages/risks/template.md` and edit it as you like. In order to find it and view the page on the site, you need to create a navigation link. Here is how you do that:
1. Create a `permalink` in the header of the new file you created. This is the URL extension that corresponds to the page. For example, `permalink: /risks/fire/` corresponds to `woodwellrisk.github.io/risks/fire`.
2. Then, go into `_data/navigation.yml` and copy and paste a `title` and `url` line. Rename the title (what will appear on the sidebar) and change the url to match `permalink`.

## Acknowledgements
This repository contains code from the `minimal-mistakes` Jekyll theme. Copyright (c) 2013-2024 Michael Rose and contributors, distributed under a MIT License.