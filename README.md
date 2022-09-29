# README

This is my beginning of learning Ruby on rails.
This is a simple to do apps.

---

* Ruby version:
    3.1.2
* Rails version:
    7.0.4
* System dependencies

* Configuration
```
bundle install
```
* Database creation
```
rails db:create
```
* Database initialization
```
rails db:migrate
```
* How to run the test suite
```
rails server
```

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

I deployed this project into Heroku. Process is below:

Within the Gemfile remove:

```
gem 'sqlite3'
```
And replace it with:
```
gem 'pg'
```
With the Gemfile updated, reinstall the dependencies:
```
bundle install
```
first have to login on heroku.
```
heroku login
```
create a new app on Heroku.
```
heroku create app_name
```
initialize git
```
git init
```
```
heroku git:remote -a app_name
```

```

```

