## Pages Contribution Guidelines

These are the files for the codes and methods website of Woodwell Climate Research Center Risk group. If you are a member of the organization, you can easily contribute.

This website framework is based on a fork of minimal-mistakes, which is a Jekyll theme framework. 

You can edit files directly in the Github editor, however it is not recommended. You should clone this repository onto your machine and make any edits/additions there. You can then add, commit and push your changes. Once Github receives your pushed changed, it will automatically rebuild and deploy the website. If this fails for whatever reason, a red x will eventually appear on the repository. The website will always be rendered as the last working version, so errors aren't a huge problem if dealt with quickly.

To avoid accidentally pushing errors to the website, you can run a local server and open it in your browser. To set this up, follow the instructions on this [GitHub Pages explainer](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll). If everything is working, you can use this command to see a live version of the site as you make changes:
```
bundle exec jekyll serve
```

### File Structure
Here are some important bits of the file structure:

1. **Webpage Markdown Files**: Each webpage is a markdown file and these are found in `_pages/`, with the exception of `index.md` in the root directory. This file is the home page.
2. **Image Files**: These are kept in `/assets/images/` and subdirectories.
3. **Navigation Bars**: You can edit vertical and horizontal navigation bars using the `_data/navigation.yml`.

### Editing Webpages
To edit an existing webpage, just edit its corresponding markdown file in `_pages/`.

### Adding new webpages
Make a copy of `_pages/risks/template.md` and edit it as you like.

To create a sidebar navigation link for the page:

1. Name the `permalink` in the file header to the name of the file. This is the URL extension that corresponds to the page, e.g. `permalink: /risks/fire/` corresponds to `woodwellrisk.github.io/risks/fire`.
2. Go into `_data/navigation.yml`.
3. Copy and paste a `title` and `url` line. Rename the title (what will appear on the sidebar) and change the url to match `permalink`.

### Images
