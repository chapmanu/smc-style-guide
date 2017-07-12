# smc-style-guide
A guide for styling and design best practices promoted by the Strategic Marketing and Communications department.

### Installation
- Clone this repository
- `gem install jekyll`
- `bundle install`
- See [Jekyll's Documentation](https://jekyllrb.com/docs/home/) for more help if needed

### Running Locally
- `bundle exec jekyll serve`

NOTE: This creates a `_site` folder in your local repository that puts your static site together. Any changes in the `_site` folder are only temporary. If you want to make changes, change them in the source folders outside of `_site`. If you want to make changes to the `config.yml` file then you need to exit and rerun the command above to see those changes.

### About This Style Guide And How It Works
- This style guide is created from jekyll and is currently using the default minima theme
- The files found in this repository under the `_layouts`, `_includes`, and `assets` folders are customized files
- Jekyll first looks inside this repository before checking its default files
- Default file configurations can be found with the command `open $(bundle show minima)`

### Adding Pages
- In the `_pages` folder create a markdown file for your new page with the following:
```
---
layout: page
title: page_title_goes_here
permalink: /permalink_goes_here/
---

{% include file_name.html %}
```
- In the _includes folder create the file you plan to include with the necessary html

### Adding SCSS and CSS files
- In the `assets` folder create your SCSS file
- If you plan to import other files into it you need to add the following at the top of the file [source](https://jekyllrb.com/docs/assets/):
```
---
---
``` 
- Be sure to link any new SCSS and CSS files to the `head.html` file in the `_includes` folder