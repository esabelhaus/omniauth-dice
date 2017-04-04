require 'psych' # Fix double-load bug when requiring yaml
require 'yaml'
if File.exist?('config/gem_sources.yml')
  YAML.load_file('config/gem_sources.yml').each do |gem_source|
    puts "Loading gem source: #{gem_source}"
    source gem_source
  end
else
  source 'https://rubygems.org'
end

gem 'cert_munger', '~> 0.2', path: '~/workspace/general_projects/cert_munger'
gem 'dnc', '~> 0.2', path: '~/workspace/general_projects/dnc'
# Specify your gem's dependencies in omniauth-dice.gemspec
gemspec
