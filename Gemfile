source 'https://rubygems.org'
#source "https://rubygems.org"

# gem "rails"
gem "rspec"
gem "ci_reporter"
gem "simplecov"
gem "simplecov-csv"

gem 'activerecord', '>= 4.0.0'

group :test do
  gem 'rake'

  case ENV['DB']
  when 'pg'
    gem 'pg'
  when 'mysql'
    gem 'mysql2'
  else
    gem 'sqlite3'
  end

  gem 'minitest', '>= 3'
end

gemspec
