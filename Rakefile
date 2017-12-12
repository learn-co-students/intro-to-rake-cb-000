namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hola'
  task :hola do
    puts "hola de Rake!"
  end
end

task :environment do
  require_relative './config/environment'
end

namespace :db do
  desc 'migrate'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'seed the database'
  task :seed do
    require_relative './db/seeds.rb'
  end
end
