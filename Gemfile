source "https://rubygems.org"

ruby ">= 3.3"

# Match the versions used by GitHub Pages so that local rendering is faithful.
gem "github-pages", "= 232", group: :jekyll_plugins

# Ruby 3 no longer includes WEBrick, which Jekyll uses for its local server.
gem "webrick", "~> 1.9"

# Used by the GitHub Metadata plugin for resilient API requests during local builds.
gem "faraday-retry", "~> 2.0", group: :development

# Ruby 3.4 lacks a standalone erb gem.
gem "erb", "~> 6.0"
