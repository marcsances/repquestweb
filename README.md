# RepQuest website

Based on [YAT](https://github.com/jeffreytse/jekyll-theme-yat/).

## Installation

There are three ways to install:

- As a [gem-based theme](https://jekyllrb.com/docs/themes/#understanding-gem-based-themes).
- As a [remote theme](https://blog.github.com/2017-11-29-use-any-theme-with-github-pages/) (GitHub Pages compatible).
- Forking/directly copying all of the theme files into your project.

### Gem-based Theme Method

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "jekyll-theme-yat"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-theme-yat
```

And then execute:

```bash
$ bundle
```

Or install it yourself as:

```bash
$ gem install jekyll-theme-yat
```

### Remote Theme Method with Jekyll Remote Theme Plugin

Remote themes are similar to Gem-based themes, but do not require `Gemfile` changes or whitelisting making them ideal for sites hosted with GitHub Pages.

To install:

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "jekyll-remote-theme", group: :jekyll_plugins
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
# theme: owner/name --> Don't forget to remove/comment the gem-based theme option
remote_theme: "jeffreytse/jekyll-theme-yat"

# Add the following to activate the plugin
plugins:
  - jekyll-remote-theme
```

And then execute:

```bash
$ bundle
```

### Forking/Cloning the project

You need to update the option of github workflow file `.github/workflows/build-jekyll.yml`, especially to ensure the value of `jekyll_baseurl` is correct.

### GitHub Pages without limitation

GitHub Pages runs in `safe` mode and only allows [a set of whitelisted plugins/themes](https://pages.github.com/versions/). **In other words, the third-party gems will not work normally**.

To use the third-party gem in GitHub Pages without limitation:

Here is a GitHub Action named [jekyll-deploy-action](https://github.com/jeffreytse/jekyll-deploy-action) for Jekyll site deployment conveniently. 👍

## Usage

Add or update your available layouts, includes, sass and/or assets.

## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

When your theme is released, only the files in `_data`, `_layouts`, `_includes`, `_sass` and `assets` tracked with Git will be bundled.
To add a custom directory to your theme-gem, please edit the regexp in `jekyll-theme-yat.gemspec` accordingly.

## Contributing

Issues and Pull Requests are greatly appreciated. If you've never contributed to an open source project before I'm more than happy to walk you through how to create a pull request.

You can start by [opening an issue](https://github.com/jeffreytse/jekyll-theme-yat/issues/new) describing the problem that you're looking to resolve and we'll go from there.
##
## License

This theme is licensed under the [MIT license](https://opensource.org/licenses/mit-license.php) © JeffreyTse.

<!-- External links -->

[jekyll]: https://jekyllrb.com/
[yat-git-repo]: https://github.com/jeffreytse/jekyll-theme-yat/
[yat-live-demo]: https://jeffreytse.github.io/jekyll-theme-yat/
[jekyll-spaceship]: https://github.com/jeffreytse/jekyll-spaceship
[jekyll-seo-tag]: https://github.com/jekyll/jekyll-seo-tag
[jekyll-sitemap]: https://github.com/jekyll/jekyll-sitemap
[jekyll-feed]: https://github.com/jekyll/jekyll-feed
[highlight-js]: https://github.com/highlightjs/highlight.js
[photoswipe-5]: https://photoswipe.com/
