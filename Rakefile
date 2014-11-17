#!/usr/bin/env rake
require 'bundler/gem_tasks'
require 'rake/testtask'
require 'ci/reporter/rake/rspec' 
require 'rspec/core/rake_task'

RSpec::Core::RakeTask.new(:spec => ["ci:setup:rspec"])
#RSpec::Core::RakeTask.new(:spec => ["ci:setup:rspec"])

Rake::TestTask.new do |t|
  t.libs = ["test"]
  t.pattern = "test/**/*_test.rb"

  # also warn about bad practices and such
  t.ruby_opts = ['-w']
end

task :default => :test
