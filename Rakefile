namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hello to the terminal'
  task :hola do
    puts "hola de Rake!"
  end

  desc 'outputs goodbye to the terminal'
  task :goodbye do
    puts "goodbye from Rake!"
  end

  desc 'outs a scream to the terminal'
  task :ahh do
    puts "AAAAHHHHHHH"
  end
end

namespace :db do

  desc 'migrates changes to the database'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'establishes a database connection'
  task :environment do
    require_relative './config/environment'
  end

  desc 'seed the database with some dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end

  desc 'drop into the Pry console'
  task :console => :environment do
    Pry.start
  end

end
