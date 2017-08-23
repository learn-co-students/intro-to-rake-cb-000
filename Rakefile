
namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hola from the terminal'
  task :hola do
    puts "hola de Rake!"
  end
end

namespace :db do
  desc 'create the students table in the database'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'populate the database table with dummy data'
  task :seed do
    require_relative './db/seeds'
  end
end

desc 'load the envionment'
task :environment do
  require_relative './config/environment'
end
