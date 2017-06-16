# The Cloud Glossary
http://glossary.cfapps.io

A glossary of terms for cloud technologies and Cloud Foundry.

## Adding a new term
The glossary app uses [Jekyll](https://jekyllrb.com), so adding a term is as easy as creating a markdown file in the `terms` directory. The structure look like this:

```
---
title: Raccoontainer
action: does a thing (keep this short)
---

A [container](/container/) runtime that looks through your trash directory for resources
```

To preview your changes, run Jekyll:

```
$ gem install jekyll bundler
$ bundle exec jekyll serve
```

## Deploy

```
jekyll build
cf push <app_name> -p _site
```
