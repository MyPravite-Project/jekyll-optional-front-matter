# Jekyll Optional Front Matter

A Jekyll plugin to make front matter optional for Markdown files

## What it does

Out of the box, Jekyll requires that any markdown file have YAML front matter (key/value pairs separated by two sets of three dashes) in order to be processed and converted to HTML.

While that behavior may be helpful for large, complex sites, sometimes it's easier to simply add a plain markdown file and have it render without fanfare.

This plugin does just that. Any Markdown file in your site's source will be treated as a Page and rendered as HTML, even if it doesn't have YAML front matter. 

## Usage

1. Add the following to your site's Gemfile:

  ```ruby
  gem 'jekyll-optional-front-matter'
  ```

2. Add the following to your site's config file:

  ```yml
  gems:
    - jekyll-optional-front-matter
  ```

## Disabling

Even if the plugin is enabled (e.g., via the `:jekyll_plugins` group in your Gemfile) you can disable it by adding the following to your site's config:

```yml
require_front_matter: true
```