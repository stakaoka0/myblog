# My blog  
This is my blog.  
The template of this project was forked from ['bencentra/centrarium'](https://github.com/bencentra/centrarium).

## Running locally
To test locally, run the following in your terminal:

```
cd /PATH/TO/LOCAL_REPO/
bundle install
bundle exec jekyll serve --port <your_port_number>
```

Open the page in your browser.  

## Configuration

All configuration options can be found in `_config.yml`.

## Adding New Posts
To add new posts, simply add a file in the `_posts/` directory that follows the convention `YYYY-MM-DD-name-of-post.md` and includes the necessary front matter. 

## Updating Header and Footer Links

Links in the header and footer are auto-generated. Links will be made for all files marked `category: page`, that have a title, and have the custom `main_nav` front-matter variable set to `true`. You can modify the rules for link generation in `_layouts/nav_links.html`.

## Updating Styles

If you want change the CSS of the theme, you'll probably want to check out these files in the `_sass/` directory:

* `base/_variables.scss`: Common values found throughout the project, including base font size, font families, colors, and more.
* `base/_typography.scss`: Base typography values for the site (see `typography.html` for a demonstration)
* `_layout.scss`: The primary styles for the layout and design of the theme.

### Important Variables

Here are the important variables from `base/_variables.scss` you can tweak to customize the theme to your liking:

* `$base-font-family`: The font-family of the body text. Make sure to `@import` any new fonts!
* `$heading-font-family`: The font-family of the headers. Make sure to `@import` any new fonts!
* `$base-font-size`: The base font-size. Defaults to $em-base from Bourbon (`bourbon/settings/_px-to-em.scss`).
* `$base-font-color`: The color for the body text.
* `$action-color`: The color for links in the body text.
* `$highlight-color`: The color for the footer and page headers (when no cover image provided).