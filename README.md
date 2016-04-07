# Sample web site

This repository contains a template for a sample research software
project web site. 

To view the web site, visit http://showyourworking.github.io/sample-site.

The site is written in HTML and
[MarkDown](http://daringfireball.net/projects/markdown/syntax), uses
[Jekyll](http://jekyllrb.com/) templates and is rendered via [GitHub
pages](https://pages.github.com/).

---

## Using the site

This site is a **template** - it cannot be used as-is and requires
customisation to your specific requirements.

If you wish to use it you should:

* Read, and work through, [GitHub pages](https://pages.github.com/).
* Clone this repository.
* Edit the configuration settings in `_config.yml`.
* Check and, if necessary, update the pages in `_includes` and 
  `_layout`.
* Check and update every single `.md` file.

Information on cloning, editing, and previewing the web site now follow.

## Editing the web site

The following sections describe how to edit and preview the web site.

### Install Git

```
sudo apt-get install -y git
```

### Fork and clone this repository

* [Sign in](http://github.com/login) to GitHub.
* [Fork](https://github.com/softwaresaved/sample-site/fork) this repository.
* Start Git Bash.
* Clone your fork onto your computer:


```
git clone http://USERNAME@github.com/USERNAME/sample-site.git
```

* Fetch the gh-pages branch, the branch which GitHub pages expects the web pages to be in, and check it out:

```
cd sample-site
git fetch gh-pages
git origin fetch gh-pages
git fetch origin gh-pages
git checkout gh-pages
```

### Set up Jekyll

It is useful to set up Jekyll on your computer so you can preview your changes before commiting and pushing them.

Install Ruby 2.0+ and Ruby development kit:

```
sudo apt-get install -y ruby2.0 ruby2.0-dev
```

Install Ruby bundler Gem:

```
sudo gem2.0 install bundler
```

Install gems required by the web site, including the gh-pages gem:

```
gem install bundler
```

### Edit pages

* Edit pages using your favourite editor.
* Preview how the pages will look on the web site:

```
bundle exec jekyll serve
```

* Browse to http://localhost:4000/sample-site
* When happy, commit your changes and push:

```
git commit -m "... ... ..."
git push origin gh-pages
```

* Create a pull request from your fork on GitHub to this repository.

---

## Hints and tips

### Page format

* Pages can be written in HTML or MarkDown.
* Level 1 headings  (`<h1>` in HTML and `#` in MarkDown) should be
  avoided on pages. 

### MarkDown page headers

* MarkDown pages should have a header of the form:

```
---
layout: page
title: TITLE
root: PATH_TO_ROOT_FOLDER
---
```

```
---
layout: page
title: Example Page
root: .
---
```

### Relative links

* Relative links between MarkDown pages are allowed but use a .html
  suffix e.g. 

```
[Copyright and licence](./CopyrightLicence.html)
```

### Page-specific contents

* Page-specific contents with links down to sections are supported for
  level 2 (`<h2>` in HTML and `##` in MarkDown) headings.

### Images

* Put images in sub-directories of assets/.
* Link to them using e.g.

```
[Some image](/assets/somedirectory/someimage.jpg)
```

* For inline images:

```
![Image description](/assets/somedirectory/someimage.jpg)
```

### Command-line, code and file excerpts

Enclose multi-line excerpts in `~~~` `~~~` delimiters.

### Site map 

* Site map indexes level 2 (`<h2>` in HTML and `##` in MarkDown) and
  level 3 (`<h3>` in HTML and `###` in MarkDown) headings.

### Site-wide configuration

* Site-wide configuration properties are in [_config.yml](./_config.yml).
* A configuration property, NAME, can be referenced in a page using:

```
{{ site.NAME }}
```

```
For support, contact {{ site.email }}.
```

* Project-specific properties can be defined.
* [_config.yml](./_config.yml) baseurl holds the sub-path of the web
  site. This should match the name of the GitHub project hosting the
  web site e.g. sample-site.

### Non-UTF-8 characters

* Jekyll does not like non-UTF-8 characters. These can be stripped out
  on Windows using Git Bash, via:

```
# Purge the characters.
iconv -f utf-8 -t utf-8 -c before.md > after.md
# Compare the files to see what was replaced.
diff before.md after.md
```
