# content.supply

[![Circle CI](https://circleci.com/gh/newatoms/contentsupply.svg?style=svg&circle-token=47cd8195c9d5e8668db4aeaf2b445d3099497fc2)](https://circleci.com/gh/newatoms/contentsupply)

This is the [content.supply](http://content.supply) website rendered out using GH-Pages

## Installation steps

The site runs on [GitHub-Pages](https://pages.github.com/), so in order to locally see what the server is going to render you need the same software installed as on the server.

GitHub-Pages runs their own modified version of static site generator named [Jekyll](http://jekyllrb.com/docs/github-pages/) named [Pages-Gem](https://github.com/github/pages-gem).

Open a command line interface (e.g. Terminal.app on OSX) and cd to the base directory of this application. Then, run:

	gem install github-pages

<img src="https://octodex.github.com/images/labtocat.png" width="100">

## Run locally

Open a command line interface (e.g. Terminal.app on OSX) and cd to the base directory of this application. Then, run:

	$ jekyll serve

The web application will be running within a second or two on http://localhost:4000. If you prefer to run the application on a custom http port, use the -P flag:

	$ jekyll serve --watch -P 8000

## Add a section to the homepage

All the sections on the homepage are MarkDown files in the folder `_homepage/` and in the subfolder of the relevant language. The files need the following FrontMatter:

```yaml
---
layout: section # The template used to render this
order: 50 # The lowest order is rendered at the top
---
```
## [The Content Guide](the-content-guide)

This guide is an organic document that has to grow and increases quality with time. Did you learn anything which involves creating content? Then this is your space to add your findings. You can of course use it as a source to consult. 
