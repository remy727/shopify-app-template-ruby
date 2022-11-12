### Steps
- Clone [shopify-app-template-ruby](https://github.com/remy727/shopify-app-template-ruby)
- Update `SHOPIFY_API_KEY` in `heroku.yml`
- Add Heroku Addons
  * Heroku Postgres
  *
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