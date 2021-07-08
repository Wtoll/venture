# Venture

[![venture](https://img.shields.io/badge/Hugo--Themes-@Venture-blue)](https://themes.gohugo.io/themes/venture/)

Venture is a bold, minimalist theme for Hugo inspired by [avc.com](https://avc.com).

## To Do

This theme is in a MVP stage, thus it is not entirely complete. The following is a list of things that need to be addressed before it is feature-full.
- [ ] The archives page ([gohugoio/hugo#448](https://github.com/gohugoio/hugo/issues/448))
- [ ] List pages that aren't gross
- [ ] Better left header content configuration
- [ ] Responsive header on mobile

## Features

The Venture theme includes a wide variety of helpful customization features to allow you to configure your site however you like.

### Profile Picture

By setting the config variable `params.pfp` you can define a profile picture to be included in the header of the page. For testing purposes the theme includes the `images/blank.png` file which can be used as a temporary, blank profile picture. When the variable is not set a profile picture will not be included in the header.

###### In `config.toml`
```toml
[params]
  pfp = "images/blank.png"
```

### Accent Color

The `params.accent_color` variable can be used to define a specific color as an accent on the page. This color is used for the hover of headers, the color of links, the fill of some svg buttons, and more. When not set the theme defaults to the color `#729426`

###### In `config.toml`
```toml
[params]
  accent_color = "#c64cb2"
```

### Built-In About Page

The Venture theme includes support for a static page with information just about you. To create an about page create the file `content/about/_index.md` with the content you want included on your "about" page.

The theme will magically do the rest and include a link to the about page in the header.

### Copyright Callout

By setting the config variable `params.copyright` you can define a custom copyright callout to go in the footer of every page. When this variable is not set the theme will simply not include a copyright callout.

###### In `config.toml`
```toml
[params]
  copyright = "&copy; Your Name Here 2021"
```

### Header Links

Additional header links can be defined by using the `menu.main` variable built into Hugo. For more information on how Hugo's menu system works check [here](https://gohugo.io/content-management/menus/).

```toml
[menu]
  [[menu.main]]
    name = "Twitter"
    url = "https://twitter.com/jack"
    weight = 1
```
