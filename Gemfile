# frozen_string_literal: true

source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby '3.0.3'

gem 'rails', '~> 6.1.4', '>= 6.1.4.1'
gem 'puma', '~> 5.0'
gem 'pg', '~> 1.2', '>= 1.2.3'
gem 'redis', '~> 4.0'
gem 'hiredis', '~> 0.6.3'
# gem 'bcrypt', '~> 3.1.7'
# gem 'image_processing', '~> 1.2'
gem 'bootsnap', '>= 1.4.4', require: false
# gem 'rack-cors'
gem 'figaro', '~> 1.2'
gem 'sidekiq', '~> 6.3', '>= 6.3.1'

group :development, :test do
  gem 'byebug', platforms: %i[mri mingw x64_mingw]
  gem 'pry-byebug'
  gem 'pry-rails'
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
