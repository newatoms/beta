# content.supply

This is the [content.supply](http://content.supply) website rendered out using GH-Pages

## Add a section to the homepage

All the sections on the homepage are MarkDown files in the folder `_homepage`. The files need the following FrontMatter

```yaml
---
title: All plans include # Title of the section
layout: section # The template used to render this
order: 50 # The lowest order is rendered at the top
id: features # This is used for design purposes
---
```
