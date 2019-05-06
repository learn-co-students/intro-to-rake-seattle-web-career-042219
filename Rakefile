
namespace :greeting do
  desc 'outputs hello to the terminal'
    task :hello do
      puts "hello from Rake!"
    end
  desc 'outputs hola to the terminal'
    task :hola do
      puts 'hola de Rake!'
    end
end

desc 'puts console string'
  task :console do
    puts "Make sure you have a 'console' rake task"
  end

desc 'set up environment'
  task :environment do
    require_relative './config/environment'
  end

namespace :db do
  desc 'migrate'
    task :migrate => :environment do
      Student.create_table
  end
  desc 'seed the database with some dummy data'
    task :seed do
      require_relative './db/seeds.rb'
  end
end
