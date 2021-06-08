$ rails new task_manager -T -d="postgresql" --skip-spring --skip-turbolinks  
cd task_manager   
$ bundle install  
rails db:create  
rails s  

$ rails generate migration CreateTask title:string description:string  
$ rails db:migrate  

$ rails dbconsole  

bundle exec rspec

rails g migration AddArtistsToSongs artist:references
