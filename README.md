# docker-ruby-rails
Starting point for new Ruby/Rails on Docker

# Includes
ruby:2.6.10
rails: 5.2.6.3
mariadb: myapp_db
phpmyadmin: myapp_phpmyadmin

# WARNING! 
This README will be overwritten once you start

# Build
* docker compose run --no-deps web rails new . --force --database=postgresql
* docker compose build
* docker compose up
* replace database.yml with actual_database.yml
* docker compose run web rake db:create
* visit localhost:3000
