```language: ruby 
rbenv:
- 2.5.3
addons:
  postgresql: 9.6
before_install:
  nvm install --lts
script:
- bundle exec rails db:{create,migrate} RAILS_ENV=test
- bundle exec rspec    



deploy:
  provider: heroku
  api_key:
    secure: <api_key>
  app: curious-dawn-777
  on:
    repo: lalalala/yardsourcing-engine  
    
    
     
  run: rails db:migrate
