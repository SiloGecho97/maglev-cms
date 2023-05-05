# Maglev CMS demo

[Maglev](https://docs.maglev.dev/)

# How To Run

To solve vite-ruby issue

```
export VITE_RUBY_SKIP_COMPATIBILITY_CHECK=true
```
or export .env file

Maglev depends on ActiveStorage for the content asset uploading. So you need to setup ActiveStorage like this:

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
