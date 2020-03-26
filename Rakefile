# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

# require_relative 'config/application'

# Rails.application.load_tasks

# Load DSL and set up stages
require "capistrano/setup"

# Include default deployment tasks
require "capistrano/deploy"

# Load the SCM plugin appropriate to your project:
#
# require "capistrano/scm/hg"
# install_plugin Capistrano::SCM::Hg
# or
# require "capistrano/scm/svn"
# install_plugin Capistrano::SCM::Svn
# or
require "capistrano/scm/git"
install_plugin Capistrano::SCM::Git

# Include tasks from other gems included in your Gemfile
#
# For documentation on these, see for example:
#
#   https://github.com/capistrano/rvm
#   https://github.com/capistrano/rbenv
#   https://github.com/capistrano/chruby
#   https://github.com/capistrano/bundler
#   https://github.com/capistrano/rails
#   https://github.com/capistrano/passenger
#
#START_HIGHLIGHT
require "capistrano/rvm"
#END_HIGHLIGHT
# require "capistrano/rbenv"
# require "capistrano/chruby"
#START_HIGHLIGHT
require "capistrano/bundler"
#END_HIGHLIGHT
#START_HIGHLIGHT
require "capistrano/rails/assets"
#END_HIGHLIGHT
#START_HIGHLIGHT
require "capistrano/rails/migrations"
#END_HIGHLIGHT
#START_HIGHLIGHT
require "capistrano/passenger"
#END_HIGHLIGHT

# Load custom tasks from `lib/capistrano/tasks` if you have any defined
Dir.glob("lib/capistrano/tasks/*.rake").each { |r| import r }
