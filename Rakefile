namespace :greeting do
  desc 'output hello'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'output hola'
  task :hola do
    puts "hola de Rake!"
  end
end

namespace :db do
  desc 'access environment'
  task :environment do
    require_relative './config/environment.rb'
  end

  desc 'migrate'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'seeding'
  task :seed do
    require_relative './db/seeds.rb'
  end
end



desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end
