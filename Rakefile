namespace :greeting  do
desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end
desc 'outputs halo to the terminal'
task :hola do
  puts "hola de Rake!"
end
end
namespace :db do
  desc 'environment initalization'
  task :migrate => :environment do
    Student.create_table
  end
  task :environment do
    require_relative './config/environment'
  end
  desc "seed db "
  task :seed  do
    require_relative './db/seeds.rb'
  end
end
