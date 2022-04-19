# README

Ruby on Rails.

Currently hosted on Heroku (Puma) webserver.

Available at: https://sorour-rails-sample-app.herokuapp.com/

* Developed with current Ruby version `ruby 3.1.1p18`. Can be checked locally by running the `ruby -v` command.

* System dependencies include Heroku for production deployment with the following command: `git push heroku main` 

* Configuration

* Database creation is with `sqlite3` in development and `postgres` in production 

* Database initialization. To reset the DB on production, run the following command: 

```
heroku pg:reset --confirm sorour-rails-sample-app
heroku run rake db:migrate
heroku restart
```

* Run the tests using `bundle exec rake test` or individually test types with `bundle exec rake test:integration`. Can also be run with the following command: `rake test`

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
