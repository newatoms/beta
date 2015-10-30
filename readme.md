# content.supply
This is the [content.supply](http://content.supply) website rendered out using GH-Pages

## Installation steps

Open a command line interface (e.g. Terminal.app on OSX) and cd to the base directory of this application. Then, run:

	$ sudo gem install jekyll
	
Oops, that's it! Amazing huh?

## Run locally

Open a command line interface (e.g. Terminal.app on OSX) and cd to the base directory of this application. Then, run:

	$ jekyll serve

The web application will be running within a second or two on http://localhost:4000. If you prefer to run the application on a custom http port, use the -P flag:

	$ jekyll serve -P 8000

## Add a section to the homepage

All the sections on the homepage are MarkDown files in the folder `_homepage`. The files need the following FrontMatter

```yaml
---
layout: section # The template used to render this
order: 50 # The lowest order is rendered at the top
id: features # This is used for design purposes
---
```
