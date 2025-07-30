source "https://rubygems.org"


gem 'jekyll'
gem 'kramdown-parser-gfm'
gem 'webrick'
gem "minimal-mistakes-jekyll"


group :jekyll_plugins do
  gem 'jekyll-feed'
  gem 'jekyll-sitemap'
  gem 'jekyll-seo-tag'
  gem 'jekyll-paginate'
  gem "jekyll-include-cache"
end



# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end


