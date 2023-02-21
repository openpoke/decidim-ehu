# frozen_string_literal: true

source "https://rubygems.org"

ruby RUBY_VERSION

# DECIDIM_VERSION = "~> 0.26.3"
DECIDIM_VERSION = { git: "https://github.com/decidim/decidim", tag: "release/0.26-stable" }.freeze

gem "decidim", DECIDIM_VERSION
# gem "decidim-conferences", DECIDIM_VERSION
# gem "decidim-consultations", DECIDIM_VERSION
# gem "decidim-elections", DECIDIM_VERSION
# gem "decidim-initiatives", DECIDIM_VERSION
# gem "decidim-templates", DECIDIM_VERSION

gem "decidim-term_customizer", git: "https://github.com/openpoke/decidim-module-term_customizer"
gem "decidim-decidim_awesome", git: "https://github.com/decidim-ice/decidim-module-decidim_awesome"

gem "bootsnap", "~> 1.3"

gem "puma", ">= 5.0.0"

gem "wicked_pdf", "~> 2.1"

group :development, :test do
  gem "byebug", "~> 11.0", platform: :mri

  gem "brakeman"
  gem "decidim-dev", DECIDIM_VERSION
  gem "faker"
  gem "rubocop-faker"
end

group :development do
  gem "letter_opener_web", "~> 1.3"
  gem "listen", "~> 3.1"
  gem "spring", "~> 2.0"
  gem "spring-watcher-listen", "~> 2.0"
  gem "web-console", "~> 4.0"

  gem "capistrano", "~> 3.17", require: false
  gem "capistrano-bundler", require: false
  gem "capistrano-passenger", require: false
  gem "capistrano-rails", require: false
  gem "capistrano-rails-console", require: false
  gem "capistrano-rbenv", require: false
  gem "capistrano-sidekiq", require: false
end

group :production do
  gem "figaro", "~> 1.2"
  gem "sidekiq", "<7"
  gem "sidekiq-cron"
end
