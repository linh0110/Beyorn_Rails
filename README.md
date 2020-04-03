# Version

Ruby version: 2.7.0

Rails version: 6.0.2.1

Database management system: PostgreSQL

Database version: 12.2

Database name: blog_development

# Install and Deloyment
## Clone repository

    $ git clone https://github.com/linh0110/Beyorn_Rails
    $ cd Beyorn_Rails
    
## Check version
User ruby and rails version

    $ ruby -v #2.7.0
    $ rails -v #6.0.2.1
    
if not have to install the correct version

    $ gem install rails -v 6.0.2.1
    
## Install dependencies

    gem install bundler
    
## Install & update Gemfile

    $ bundle install
    
## Initialize the database

    $ rails db:setup #create database
    $ db:migrate #create table and data structure
    $ db:seed #create seed data

yarn : v1.22.4 if the run fails, Please run 'yarn install --check-files' to update.

# Run server

    $ rails s
    
# Run on browser
    http://localhost:3000/
