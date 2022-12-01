# Shopify App Template - Rails 7 + Heroku + Postgres

### Steps
- Clone [shopify-app-template-ruby](https://github.com/remy727/shopify-app-template-ruby)
- Install the ruby dependencies:
  ```shell
  $ cd web
  $ bundle install
  ```
- Run the [Rails template](https://guides.rubyonrails.org/rails_application_templates.html) script.
  ```shell
  $ cd web
  $ bin/rails app:template LOCATION=./template.rb
  ```
- Update `SHOPIFY_API_KEY` in `heroku.yml`
- Add Heroku Addons
  * [Heroku Postgres](https://elements.heroku.com/addons/heroku-postgresql)
  * [Heroku Data for Redis](https://elements.heroku.com/addons/heroku-redis)
- Add ENVs

  | Variable                   |
  | -------------------------- |
  | `HOST`      |
  | `RAILS_MASTER_KEY`         |
  | `RAILS_ENV`                |
  | `RAILS_SERVE_STATIC_FILES` |
  | `RAILS_LOG_TO_STDOUT`      |
  | `SHOPIFY_API_KEY`          |
  | `SHOPIFY_API_SCOPES`       |
  | `SHOPIFY_API_SECRET`       |
  | `SHOPIFY_APP_NAME`         |

- Deploy
- Run `heroku ps:scale worker=1`