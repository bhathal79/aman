# Bootstrap-BP hugo startpage

Bootstrap based Hugo startpage theme which provides out of the box best practices.
This theme is a combination of my [Bootstrap-BP hugo theme](https://github.com/spech66/bootstrap-bp-hugo-theme) and my [startpage](https://github.com/spech66/startpage).
Instead of rendering the items on-the-fly as in the startpage theme the **Bootstrap-BP hugo startpage** will generate a complete single page site.

## Install the theme

With Git installed, run the following commands inside the Hugo site folder. If Hugo has not yet been installed, read the setup guide [here](https://gohugo.io/overview/installing/).

```sh
mkdir themes
cd themes
git clone https://github.com/spech66/bootstrap-bp-hugo-startpage.git
```

You can get a zip of the latest version of the theme from the [home page](https://github.com/spech66/bootstrap-bp-hugo-theme) and extract it to the themes folder.

## Theme settings

Most settings should be done with hugo specific variables. There are only a few (optional) additional `[params]`.

* `startPageColumns = true` will show the start page in a Masonry-like mode.

## Google Analytics

This theme uses the internal asynchronous template for Google Analytics tracking. You only have to provide your tracking id in your configuration file:

```yaml
googleAnalytics = "UA-123-45"
```

## Schema.org support

Provide one author to enable the Schema.org support.

```yaml
[Author]  
  name = "Sebastian Pech"
```

## Images, Open Graph and Twitter Cards

This theme uses Hugos `feature/cover` name method to set the optimized feature image. This will also be in the Twitter Cards and Open Graph block.

```yaml
# Site Config toml
title = "My hugo site"

[params]
  description = "Text about the site"
```