require 'rubygems'
require 'rake'

begin
  gem 'jeweler', '~> 1.4'
  require 'jeweler'

  Jeweler::Tasks.new do |gem|
    gem.name        = 'dm-sqlite3-adapter'
    gem.summary     = 'Sqlite3 Adapter for DataMapper'
    gem.description = gem.summary
    gem.authors     = ["Dan Kubb"]
    gem.email       = %q{dan.kubb@gmail.com}
    gem.homepage    = 'http://github.com/datamapper/dm-more/tree/master/adapters/%s' % gem.name

    gem.rubyforge_project = 'datamapper'

    gem.add_dependency 'data_objects', '~> 0.10.1'
    gem.add_dependency 'do_sqlite3', '~> 0.10.1'
    gem.add_dependency 'dm-core', '~> 0.10.3'
    gem.add_dependency 'dm-data_objects-adapter', '~> 0.10.3'

    gem.add_development_dependency 'rspec', '~> 1.3'
    gem.add_development_dependency 'yard', '~> 0.5'
  end

  Jeweler::GemcutterTasks.new

  FileList['tasks/**/*.rake'].each { |task| import task }
rescue LoadError
  puts 'Jeweler (or a dependency) not available. Install it with: gem install jeweler'
end
