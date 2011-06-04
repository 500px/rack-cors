require 'rake'
require 'rake/testtask'

desc 'Run tests'
Rake::TestTask.new(:test) do |t|
  t.pattern = 'test/*_test.rb'
  t.verbose = true
  t.warning = true
end

# ==================================================
# JEWELER TASKS
# ==================================================
begin
  require 'jeweler'
  Jeweler::Tasks.new do |gemspec|
    gemspec.name = "rack-cors"
    gemspec.summary = "Middleware for enabling Cross-Origin Resource Sharing in Rack apps"
    gemspec.email = "csyu77@gmail.com"
    gemspec.homepage = "http://github.com/cyu/rack-cors"
    gemspec.authors = ["Calvin Yu"]
    gemspec.add_dependency 'rack'
    gemspec.files.exclude 'Gemfile'
  end
  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler not available. Install it with: gem install jeweler"
end

