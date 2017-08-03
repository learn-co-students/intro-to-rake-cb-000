task :environment  do
  require_relative './config/environment.rb'
end

desc 'outputs hello to the terminal'
namespace :greeting do
  
  task :hello do
    puts "hello from Rake!"
  end

  task :hola do
    puts 'hola de Rake!'
  end
  
end


desc 'Database operations'
namespace :db do 
  task :migrate => :environment do
    Student.create_table
  end

 

  task :seed do 
    require_relative './db/seeds.rb'
  end

end
desc 'Open up the PRY console'
task :console => :environment do 
  Pry.start
end


