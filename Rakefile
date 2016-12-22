task :environment do
  require_relative './config/environment'
end

desc 'outputs hello to the terminal'
namespace :greeting do
  task :hello do
    puts "hello from Rake!"
  end

  task :hola do
    puts "hola de Rake!"
  end
end

desc "database tasks"
namespace :db do
  task :migrate => :environment do
    Student.create_table
  end

  task :seed do
    require_relative './db/seeds'
  end
end

task :console => :environment do
  binding.pry
end
