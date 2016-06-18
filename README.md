###Run this app in production
- `rake db:migrate RAILS_ENV=production`
- `rake secret` to generate a random secret
- `set  SECRET_KEY_BASE=<secret generated>`
- `set RAILS_SERVE_STATIC_FILES=true`
- `rake assets:precompile RAILS_ENV=production`
- `rails server -e production`