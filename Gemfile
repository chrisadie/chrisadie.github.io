source "https://rubygems.org"

# The "github-pages" meta-gem (latest: 232) pins jekyll-remote-theme 0.4.3,
# which caps rubyzip below 3.0 and so cannot get the fix for CVE-2026-85396
# (rubyzip path traversal, fixed in rubyzip >= 3.4.0). Instead we declare
# Jekyll and the plugins directly, matching the versions GitHub Pages uses,
# but with a jekyll-remote-theme that allows a patched rubyzip.
gem "jekyll", "= 3.10.0"
gem "kramdown", "= 2.4.0"
gem "kramdown-parser-gfm", "= 1.1.0"
gem "webrick", "~> 1.8"

gem "rubyzip", ">= 3.4.0"

gem "tzinfo-data"
gem "wdm", "~> 0.1.0" if Gem.win_platform?

# If you have any plugins, put them here!
group :jekyll_plugins do
  gem "jekyll-remote-theme", ">= 0.6.2"
  gem "jekyll-github-metadata", "= 2.16.1"
  gem "jekyll-paginate", "= 1.1.0"
  gem "jekyll-sitemap", "= 1.4.0"
  gem "jekyll-gist", "= 1.5.0"
  gem "jekyll-feed", "= 0.17.0"
  gem "jemoji", "= 0.13.0"
  gem "jekyll-include-cache", "= 0.2.1"
end

# Command to run the site locally:
# bundle exec jekyll serve --port 4010

# Command to update the gemfile.lock file:
# bundle update
