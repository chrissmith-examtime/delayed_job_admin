delayed_job_admin
=================

Adding some simple admin features to delayed_job

This project is a mountable rails engine to provide some useful admin tools to monitor your delayed jobs queue.

Getting Started

Add the gem to your Gemfile
`gem 'delayed_job_admin'`

Run the install 
`rails g delayed_job_admin:install`

Run the migrations (adds a delayed_jobs_archive table)
`rake db:migrate`

Mount the engine in your routes.rb
`
Rails.application.routes.draw do
  ...
  mount DelayedJobAdmin::Engine => "/delayed_job_admin"
  ...
end
`

== Getting started with development (i.e. running tests)

  1. Clone the repo from GitHub git@github.com:ExamTime/ninja_access.git
  2. cd delayed_job_admin
  3. bundle install --binstubs
  5. rake db:create && rake db:migrate && rake db:test:prepare
  6. rake 
