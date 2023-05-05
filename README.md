# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

- Ruby version

- System dependencies

- Configuration

- Database creation

- Database initialization

- How to run the test suite

- Services (job queues, cache servers, search engines, etc.)

- Deployment instructions

- ...

# How To Run

TO solve vite-ruby issue

```
export VITE_RUBY_SKIP_COMPATIBILITY_CHECK=true
```

```
bundle exec rails active_storage:install
bundle exec rails db:create
bundle exec rails db:migrate
```

Setup Maglev

```
bundle exec rails g maglev:install
bundle exec rails g maglev:hyperui:install --force
bundle exec rails maglev:create_site
```

Launch your rails app

```
bundle exec rails s
```
