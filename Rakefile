desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

namespace :greeting do
  desc 'Puts hello'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'puts hola'
  task :hola do
    puts "hola de Rake!"
  end
end

namespace :db do
  desc ''
  task :migrate => :environment do
    Student.create_table
  end

  desc 'sets up the enviornment'
  task :environment do
    require_relative './config/environment'
  end

  desc 'seed the database with some dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end
end
