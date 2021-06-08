## [Heroku notes](https://devcenter.heroku.com/articles/getting-started-with-rails5)
#### Heroku-18 is needed to work with `Rails 5.4.3`
- Specify stack when creating app:  
  `heroku create --stack heroku-18`
- To change the stack on an existing app  
  `heroku stack:set heroku-18`
- [Heroku-18 Stack](https://devcenter.heroku.com/articles/heroku-18-stack)
#### Steps to Deploy App
- Create with directory that contains rails app  
  `heroku create`
- Verify remote is running  
  `git config --list | grep heroku`
- Deploy code **never push anything but main branch**  
  `git push heroku main`
- If no errors, migrate database  
  `heroku run rails db:migrate`
#### Visit App
- Assign one **dyno** running the app  
  `heroku ps:scale web=1`
- Check the state of app's dynos  
  `heroku ps`
- Open the app in browser  
`heroku open`


`heroku run rails csv_load:all`
