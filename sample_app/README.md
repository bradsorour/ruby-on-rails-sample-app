# README

Ruby on Rails Sample App.

Currently hosted on Heroku (Puma) webserver here: https://sorour-rails-sample-app.herokuapp.com/

This sample app covers all of the major features of Rails, including;

* Models
* Views
* Controllers
* Templates
* Partials
* Filters
* Validations
* Callbacks
* Has-Many
* Security
* Testing
* Deployment

***

* Developed with current Ruby version `ruby 3.1.1p18`. Can be checked locally by running the `ruby -v` command.

* System dependencies include Heroku for production deployment with the following command: `git push heroku main` 

* Configuration

* Database creation is with `sqlite3` in development and `postgres` in production 

* Database initialization. 

To reset the DB locally, run the following command: 

```
rake db:migrate:reset
rake db:seed
```

To reset the DB on production, run the following command: 

```
heroku pg:reset --confirm sorour-rails-sample-app
heroku run rake db:migrate
heroku restart
```

* Run the tests using `bundle exec rake test` or individually test types with `bundle exec rake test:integration`. Can also be run with the following command: `rake test`

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions. Before pushing to live heroku site enable maintenance on message: `heroku maintenance:on`. 
Then run the following commands:
- `git push heroku main`
- `heroku run rake db:migrate`
- If you need to seed the db, you can run `heroku run rake db:seed`
- Then turn maintenance off with `heroku maintenance:off`

* To kill the local rails server, run the following command : `kill -9 $(lsof -i tcp:3000 -t)`

## Supplementary Resources

### Destroy without JavaScript

http://railscasts.com/episodes/77-destroy-without-javascript-revised
