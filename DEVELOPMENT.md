# Local Development

This site uses Jekyll with the Minima theme. GitHub Pages can build it as-is, but for local preview you need Bundler to install the theme and plugins listed in the Gemfile.

## Prerequisites
- Ruby (recommended 3.1–3.3). Ruby 4.0 may work but is not widely tested with all gems yet.
- Bundler: `gem install bundler`

## Install dependencies
```powershell
bundle install
```

## Run the site locally
```powershell
bundle exec jekyll serve --livereload
```
Visit http://localhost:4000

## Notes
- The theme is configured in `_config.yml` as `theme: minima`.
- If file watching is slow on Windows, the optional `wdm` gem is included.
- If you prefer to match the exact GitHub Pages environment, we can switch to the `github-pages` gem; however, it may lag behind the latest Jekyll and Ruby.
