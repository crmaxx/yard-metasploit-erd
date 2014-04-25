source 'https://rubygems.org'

# Specify your gem's dependencies in yard-metasploit-erd.gemspec
gemspec

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
  # restrict for compatibility with rest of metasploit ecosystem until it upgrades to Rails 4
  gem 'activesupport', '>= 3.2', '< 4.0.0'
  # Upload coverage reports to coveralls.io
  gem 'coveralls', require: false
  # code coverage of tests
  gem 'simplecov', require: false
end
