require "rubocop/rake_task"
require "rspec/core/rake_task"
require "cucumber/rake/task"

RSpec::Core::RakeTask.new "rspec"
RuboCop::RakeTask.new
Cucumber::Rake::Task.new "cucumber" do |t|
  t.cucumber_opts = "features --format progress"
end

task default: [
  :rubocop,
  :rspec,
  :cucumber,
]
