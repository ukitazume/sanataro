source 'http://rubygems.org'

gem 'rails', '3.2.1'

# Bundle edge Rails instead:
# gem 'rails', :git => 'git://github.com/rails/rails.git'

# uncomment if you use sqlite3
gem 'sqlite3-ruby', :require => 'sqlite3'

# Use unicorn as the web server
# gem 'unicorn'

gem 'capistrano' unless ENV['TRAVIS_RUBY_VERSION']

# To use debugger (ruby-debug for Ruby 1.8.7+, ruby-debug19 for Ruby 1.9.2+)
# gem 'ruby-debug'
# Bundle gems for the local environment. Make sure to
# put test-only gems in this group so their generators
# and rake tasks are available in development mode:
# group :development, :test do
#   gem 'webrat'
# end

gem "therubyracer"
group :development, :test do
  unless ENV['TRAVIS_RUBY_VERSION']
    gem "libnotify" if RUBY_PLATFORM.downcase =~ /linux/
    gem "rb-inotify" if RUBY_PLATFORM.downcase =~ /linux/
    gem 'ruby-debug19'
  end
  gem "cucumber-rails"
  gem "launchy"
  gem "fabrication"
end

gem 'haml-rails'

group :test do
  gem "cucumber", "= 1.1.4"
  gem "capybara-webkit"
  gem "database_cleaner"
  gem "guard-rspec"
  gem "guard-cucumber"
  gem "guard-spork"
  gem 'spork'
  unless ENV['TRAVIS_RUBY_VERSION']
    gem "growl" if RUBY_PLATFORM.downcase =~ /darwin/
    gem "rb-fsevent" if RUBY_PLATFORM.downcase =~ /darwin/
  end
  gem "simplecov"
  gem "rspec"
  gem "rspec-rails"
  gem "assert_valid_markup"
  gem "webrat"
end

gem "i18n"
if defined?(JRUBY_VERSION)
  gem "jruby-openssl"
  gem "activerecord-jdbcmysql-adapter"
else
  gem "mysql2"
end
gem 'jquery-rails'

group :assets do
  gem 'sass-rails', "~> 3.2.3"
  gem 'coffee-rails', "~> 3.2.1"
  gem 'uglifier', ">= 1.0.3"
end

gem 'settingslogic'
gem 'coffee-filter'
