# Rails TODO apps

This is my beginning of learning Ruby on rails.
This is a simple to do apps.

[Live demo](https://mur-todo-app.herokuapp.com/)

---

* Ruby version:
    3.1.2
* Rails version:
    7.0.4
* Configuration:
```
bundle install
```
* Database creation:
```
rails db:create
```
* Database initialization:
```
rails db:migrate
```
* How to run the test suite:
```
rails server
```
* Deployment instructions:

I deployed this project into Heroku. Process is below:

Within the Gemfile remove:

```
gem "sqlite3", "~> 1.4"
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
 initialize a local empty Git repository and commit
```
git init

git add .

git commit -m "commit message"
```
create a new app on Heroku.
```
heroku create app_name
```
initialize git
```
git init

heroku git:remote -a app_name
```
Deploy the code:
```
git push heroku main
```
or
```
git push heroku master
```
Migrate The Database
```
heroku run rake db:migrate
```
Deployment reference: https://devcenter.heroku.com/articles/getting-started-with-rails7

```
.
├── ...
├── test                    # Test files (alternatively `spec` or `tests`)
│   ├── benchmarks          # Load and stress tests
│   ├── integration         # End-to-end, integration tests (alternatively `e2e`)
│   └── unit                # Unit tests
└── ...
```
