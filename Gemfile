# frozen_string_literal: true

source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby '3.0.3'

gem 'rails', '~> 6.1.4', '>= 6.1.4.1'
gem 'puma', '~> 5.0'
gem 'redis', '~> 4.0'
# gem 'bcrypt', '~> 3.1.7'
# gem 'image_processing', '~> 1.2'
gem 'bootsnap', '>= 1.4.4', require: false
# gem 'rack-cors'

group :development, :test do
  gem 'pry'
  gem 'pry-rails'
  gem 'pry-nav'
  gem 'rubocop', '~> 1.23', require: false
  gem 'rubocop-performance', '~> 1.12'
  gem 'rubocop-rails', '~> 2.12', '>= 2.12.4'
  gem 'rubocop-rspec', '~> 2.6'
end

group :development do
  gem 'listen', '~> 3.3'
  gem 'spring'
end

gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
