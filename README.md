https://tony-rails-example.herokuapp.com/

###Run this app in production
- `rake db:migrate RAILS_ENV=production`
- `rake secret` to generate a random secret
- `set  SECRET_KEY_BASE=<secret generated>`
- `set RAILS_SERVE_STATIC_FILES=true`
- `rake assets:precompile RAILS_ENV=production`
- `rails server -e production`

###Deploy to heroku
- `git push heroku master`
- `heroku run rake db:migrate`
- `heroku open`
- `heroku logs --tail`
- `heroku config`
- `heroku config:set TEST=1`
- `heroku run rails console`
- `heroku pg:psql`
- `\dt`
- `\d questions`
- `heroku pg:info`

###utility commands
- `rvm use <version>`
- `rvm list`
- `rails s`
- `rails c`
- `rails new rails-example`
- `rails g model Manager name:string`
- `rails destroy model Manager name:string`
- `rails g controller home index`
- `rails g resource answer question_id:integer email:string body:text`
- `rails g mailer main_mailer notify_question_author`
- `rake -T`
- `rake db:migrate RAILS_ENV=test`
- `rake test`
- `rake secret`
- `rake routes`
- `bundle install`
- `bundle update`
- `git grep input.*email`
- `git diff`