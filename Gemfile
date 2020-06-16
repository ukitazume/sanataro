source 'http://rubygems.org'

###
### This file is for MRI
### Please see gemfiles/Gemfile.jruby for JRuby env
###

gem 'rails', '5.0.0'

# Bundle edge Rails instead:
# gem 'rails', :git => 'git://github.com/rails/rails.git'

# Use unicorn as the web server
# gem 'unicorn'


group :development, :test do
  gem "rspec-rails", ">= 2.11.0"
  gem "launchy"
  gem "fabrication"
  unless ENV['TRAVIS']
    platforms :mri_19 do
      gem 'capistrano'
      gem 'rvm-capistrano'
      gem 'debugger'
    end
  end
end


group :test do
  gem "simplecov"
  gem 'spork'
  platform :mri do
    gem "cucumber-rails", ">= 1.3.0", :require => false
    gem "capybara-webkit", ">= 0.12.1"
    gem "growl"
    gem "rb-fsevent"
    gem "webrat", ">= 0.7.3"
    gem "database_cleaner"
    gem "guard-rspec"
    gem "guard-cucumber"
    gem "guard-spork"
  end
end

platforms :ruby do
  gem "mysql2"
  gem 'sqlite3'
  gem 'pg'
end

platforms :mri do
  gem "therubyracer"
end

group :assets do
  gem 'sass-rails', '>= 5.0.5'
  gem 'coffee-rails', '>= 4.1.1'
  gem 'uglifier'
end

gem "i18n"
gem 'haml-rails', '>= 0.5.3'
gem 'jquery-rails', '>= 4.4.0'
gem 'jquery-ui-rails', '>= 2.0.1'
gem 'settingslogic'
gem 'coffee-filter'
gem 'memoist'

gem 'twitter-bootstrap-rails', '>= 2.1.3'
gem 'dalli'

