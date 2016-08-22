source ENV['GEM_SOURCE'] || 'https://rubygems.org'

group :test do
  gem 'rake'
  gem 'puppet', ENV['PUPPET_GEM_VERSION'] || '~> 3.8.0'
  gem 'rspec', '< 3.2.0'
  gem 'rspec-puppet'
  gem 'puppetlabs_spec_helper'
  gem 'metadata-json-lint'
  gem 'rspec-puppet-facts'
  gem 'rubocop', '0.40.0'
  gem 'simplecov', '>= 0.11.0'
  gem 'simplecov-console'
  gem 'coveralls', :require => false

  gem 'puppet-lint-absolute_classname-check'
  gem 'puppet-lint-leading_zero-check'
  gem 'puppet-lint-trailing_comma-check'
  gem 'puppet-lint-version_comparison-check'
  gem 'puppet-lint-classes_and_types_beginning_with_digits-check'
  gem 'puppet-lint-unquoted_string-check'
  gem 'puppet-lint-resource_reference_syntax'

  gem 'rest-client'
  gem 'webmock'
  gem 'mocha'
  gem 'fakefs'

  if RUBY_VERSION < '2.0'
    gem 'json',        '~> 1.8'
    gem 'json_pure',   '= 2.0.1'
    gem 'addressable', '= 2.3.8'
    gem 'tins',        '= 1.6.0'
  else
    gem 'json'
    gem 'tins'
  end
end

group :development do
  gem 'travis'
  gem 'travis-lint'
  gem 'puppet-blacksmith'
  gem 'guard-rake'
end

group :system_tests do
  gem 'beaker'
  gem 'beaker-rspec'
  gem 'beaker-puppet_install_helper'
end
