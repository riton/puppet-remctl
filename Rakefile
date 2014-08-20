require 'rubygems'
require 'puppetlabs_spec_helper/rake_tasks'
require 'puppet-lint/tasks/puppet-lint'   

PuppetLint.configuration.fail_on_warnings
PuppetLint.configuration.send('disable_80chars')
PuppetLint.configuration.send('disable_arrow_alignment')
PuppetLint.configuration.send('disable_class_inherits_from_params_class')
PuppetLint.configuration.ignore_paths = ["spec/**/*.pp", "pkg/**/*.pp", "tests/**/*.pp"]

task :default => [:syntax, :spec, :lint]
