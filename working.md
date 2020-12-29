# This is not pushed to origin... PLEASE keep it that way!!!

## tl;dr of how tf do I edit this file?

To add pages, make a markdown file (ie. `page1.md`) then it will show up in `charlee674.github.io/page1`.

Make sure you add appropriate yml settings in the top of your Markdown file:
```HTML
---
# Config settings here
---
```

More info: https://github.com/daattali/beautiful-jekyll#customizing-parameters-for-each-page

### I want to edit locally, how do I do it?

1. Install Jekyll and Ruby following [these steps](https://jekyllrb.com/docs/installation/)
   - If you run on Windows, you might run into some dependency issues with `tzinfo`. To solve it, download `tzinfo` manually via `gem install tzinfo-data`, append `gem 'tzinfo-data'` to your Gemfile, and then run `bundle install` in this repo before proceeding.
2. To run a development local server, run `bundle exec jekyll serve --watch` to watch updates and check your site locally. 

### I want to align images or add my own css?

Customized CSS can be added under `assets/css/other.css` and utilized in line with Kramdown syntax. For example:
```Markdown
![yesh](example.png){: .css-rule}
```

Or you can do it inline as well:
```Markdown
![image](path-to-image.jpg){: style="float: left"}
```