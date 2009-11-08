require 'rake'
require 'rake/rdoctask'

desc "Generate documentation for the Rails framework"
Rake::RDocTask.new do |rdoc|
  rdoc.rdoc_dir = 'doc/rdoc'
  rdoc.title    = "Ruby on Rails Documentation"

  # rdoc.options << '--line-numbers' << '--inline-source'
  rdoc.options << '-A cattr_accessor=object'
  rdoc.options << '--charset' << 'utf-8'
  rdoc.options << '--fmt=ri'
  # rdoc.options << '--merge'

  rdoc.template = ENV['template'] ? "#{ENV['template']}.rb" : './doc/template/dictionary.rb'

  root = '/Library/Ruby/Gems/1.8/gems'

  rdoc.rdoc_files.include(root + '/rails-2.3.2/CHANGELOG')
  rdoc.rdoc_files.include(root + '/rails-2.3.2/MIT-LICENSE')
  rdoc.rdoc_files.include(root + '/rails-2.3.2/README')
  rdoc.rdoc_files.include(root + '/rails-2.3.2/lib/{*.rb,commands/*.rb,rails/*.rb,rails_generator/*.rb}')
  rdoc.rdoc_files.include(root + '/activerecord-2.3.2/README')
  rdoc.rdoc_files.include(root + '/activerecord-2.3.2/CHANGELOG')
  rdoc.rdoc_files.include(root + '/activerecord-2.3.2/lib/active_record/**/*.rb')
  rdoc.rdoc_files.include(root + '/activerecord-2.3.2/lib/active_record/base.rb')
  rdoc.rdoc_files.exclude(root + '/activerecord-2.3.2/lib/active_record/vendor/*')
  rdoc.rdoc_files.include(root + '/activeresource-2.3.2/README')
  rdoc.rdoc_files.include(root + '/activeresource-2.3.2/CHANGELOG')
  rdoc.rdoc_files.include(root + '/activeresource-2.3.2/lib/active_resource.rb')
  rdoc.rdoc_files.include(root + '/activeresource-2.3.2/lib/active_resource/*')
  rdoc.rdoc_files.include(root + '/actionpack-2.3.2/README')
  rdoc.rdoc_files.include(root + '/actionpack-2.3.2/CHANGELOG')
  rdoc.rdoc_files.include(root + '/actionpack-2.3.2/lib/action_controller/**/*.rb')
  rdoc.rdoc_files.include(root + '/actionpack-2.3.2/lib/action_view/**/*.rb')
  rdoc.rdoc_files.exclude(root + '/actionpack-2.3.2/lib/action_controller/vendor/*')
  rdoc.rdoc_files.include(root + '/actionmailer-2.3.2/README')
  rdoc.rdoc_files.include(root + '/actionmailer-2.3.2/CHANGELOG')
  rdoc.rdoc_files.include(root + '/actionmailer-2.3.2/lib/action_mailer/base.rb')
  rdoc.rdoc_files.exclude(root + '/actionmailer-2.3.2/lib/action_mailer/vendor/*')
  rdoc.rdoc_files.include(root + '/activesupport-2.3.2/README')
  rdoc.rdoc_files.include(root + '/activesupport-2.3.2/CHANGELOG')
  rdoc.rdoc_files.include(root + '/activesupport-2.3.2/lib/active_support/**/*.rb')
  rdoc.rdoc_files.exclude(root + '/activesupport-2.3.2/lib/active_support/vendor/*')
end