source 'https://rubygems.org'

# Specify your gem's dependencies in yard-metasploit-erd.gemspec
gemspec

# This isn't in gemspec because metasploit-framework has its own patched version of 'metasploit-erd' that it needs
# to use instead of this gem.
# Generates namespace Module and Class<ActiveRecord::Base> specific ERDs for use in templates
gem 'metasploit-erd', github: 'crmaxx/metasploit-erd', branch: 'staging/rails-4.2'

group :development, :test do
  # markdown formatting for yard
  gem 'kramdown', platforms: :jruby
  # markdown formatting for yard
  gem 'redcarpet', platforms: :ruby
  # documentation
  # 0.8.7.4 has a bug where setters are not documented when @!attribute is used
  gem 'yard', '< 0.8.7.4'
end

group :test do
  # blank?
  gem 'activesupport', '>= 4.2.1'
  # Upload coverage reports to coveralls.io
  gem 'coveralls', require: false
  # code coverage of tests
  gem 'simplecov', require: false
end
