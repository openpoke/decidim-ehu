# frozen_string_literal: true

source "https://rubygems.org"

ruby RUBY_VERSION

DECIDIM_VERSION = { github: "decidim/decidim", branch: "release/0.29-stable" }.freeze

gem "decidim", DECIDIM_VERSION
gem "decidim-conferences", DECIDIM_VERSION
gem "decidim-templates", DECIDIM_VERSION
# gem "decidim-elections", DECIDIM_VERSION
# gem "decidim-initiatives", DECIDIM_VERSION
# gem "decidim-collaborative_texts", DECIDIM_VERSION

gem "decidim-decidim_awesome", github: "decidim-ice/decidim-module-decidim_awesome", branch: "release/0.29-stable"
gem "decidim-term_customizer", github: "mainio/decidim-module-term_customizer", branch: "release/0.29-stable"

gem "bootsnap", "~> 1.7"
gem "health_check"
gem "puma"
gem "rack-proxy", "~> 0.7"

group :development, :test do
  gem "byebug", "~> 11.0", platform: :mri

  gem "brakeman", "~> 5.4"
  gem "decidim-dev", DECIDIM_VERSION
  gem "faker", "~> 3.5.3"
  gem "rubocop-faker"
end

group :development do
  gem "letter_opener_web"
  gem "listen"
  gem "web-console"
end

group :production do
  gem "sidekiq"
  gem "sidekiq-cron"
end
