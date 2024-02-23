# docker-ruby-rails
Starting point for new Ruby/Rails on Docker using MariaDB

# Includes
ruby:2.6.10
rails: 5.2.6.3
mariadb: myapp_db
phpmyadmin: myapp_phpmyadmin

# WARNING! 
The README will be overwritten once you start. See instructions.txt.

# Build
* docker compose run --no-deps web rails new . --force --database=mysql
* docker compose build
* in actual_database.yml rename the databases as required
* in docker-compose.yml rename the app as required
* replace database.yml with actual_database.yml
* docker compose run web rake db:create
* docker compose up
* visit localhost:3000
* delete instructions.txt & actual_database.yml
