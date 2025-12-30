## About

https://ruby-on-rails-buildeployship.onrender.com/

This README would normally document whatever steps are necessary to get the
application up and running.
- Ruby version
- System dependencies
- Configuration
- Database creation
- Database initialization
- How to run the test suite
- Services (job queues, cache servers, search engines, etc.)
- Deployment instructions

## Architecture
- Web Service: Render (Ruby/Rails)
- Database: PostgreSQL 18 (Render)
- Region: Virginia (US East)

## Environment Variables
| Variable | Description |
|----------|-------------|
| DATABASE_URL | PostgreSQL connection string |
| RAILS_MASTER_KEY | Decrypts credentials |

## Deployment
Automatic deploys on push to `main` branch via Render.

## Troubleshooting
- SQLite doesn't work on cloud platforms due to ephemeral filesystems
- The `cable` database config is required for Action Cable in Rails 8
- Environment variables link separate services (web + database)
- Build commands can run migrations: `bundle exec rake db:migrate`
