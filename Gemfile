# frozen_string_literal: true

source "https://rubygems.org"

gemspec

group :development do
  if RUBY_VERSION >= "2.0.0"
    gem "byebug"
    gem "pry-byebug"
  else
    gem "pry-debugger"
  end

  gem "benchmark-ips"
end

group :test do
  gem "rake",     "~> 12.0"
  gem "rspec",    "~> 3.5.0"
  gem "rubocop",  "~> 0.51", require: false if RUBY_VERSION >= "2.1"
  gem "string-scrub" if RUBY_VERSION <= "1.9.3"
end
