# README

https://guides.rubyonrails.org/getting_started.html

* Notes

	- The two major guiding principles of Rails Philosophy are: 
		+ Don't Repeat Yourself:
		"Every piece of knowledge must have a single, unambiguous, authoritative representation within a system."
		and
		+ Convention over configuration:
		Rails has opinions about the best way to do many things in a web application, and defaults to this set of conventions

	- To install rails you need:
		+ Ruby >= 2.5.0
		+ SQLite3 
		+ Node.js >= 8.16.0
		+ yarn

	- rails folders app:
		controllers, models views etc.

	- rails folders bin:
		rails scripts to start, setup, update deploy or run your app
	
	- rails folders config:
		config fo apps, routes, database etc.

	- rails folders config.ru:
		rack config for rack based servers

	- rails folders db:
		db schema an migrations

	- rails folders lib:
		extended modules for your application
	
	- rails folders log:
		application log files
	
	- rails folders public:
		only outside viewable folder, contains static files and compiled assets
	
	- rails folders storage:
		active storage files for disk service

	- rails folders test:
		unit tests, fixtures etc

	- rails folders tmp:
		temp files like cache and pid files

	- rails folders vendor:
		a place for 3rd party code e.g. vendored gems

	

	- rails files Gemfile:
		specify gem dependencies, used by bundler gem
	
	- rails files Gemfile.lock:
		specifies exact gem versions used, should be added kept in repo

	- rails files package.json:
		npm dependencies used by yarn

	- rails files Rakefile:
		locates ans loads tasks to run from commandline,
		tasks should be added to lib/tasks instead of here

	- rails files README.md:
		brief instruction manual for your application

	- rails files .gitignore:
		tells git which files or patterns to ignore

	- rails files .ruby-version:
		specifies the default ruby version

	- rails files .ruby-gemset
		specifies the default ruby gemset

	
	- Default web server
		puma 

	- Default rails home location
		http://localhost:3000

	- Rails picks up changes made to files
		automatically

	- To get rails to say "hello", at minimum you need
		A controller and a view

	- A rails controller
		Receives specific requests for the application

	- Rails routing decides
		which controller receives which requests,
		more than one per controller - actions

	- Rails action
		Collects info to provide to a view

	- Rails view
		written in embedded ruby, displays info in human readable format, 
		processed by the request cycle before returned to the user

	- Rails generate controller command does the follow
		creates controller file
		adds route
		creates view
		creates controller tests
		creates helper
		creates scss assests
		creates index action

	- route added for controller action is
		get 'welcome/index'

	- to point home page of app to a controller action
		root 'welcome#index'

	- route file uses a
		Domain Specifc langauge (DSL) e.g. HTML

	- a resource is
		a collection of similar objects such as articles,
		people, or animals












* Commands


	- To install rails:
		+ gem install rails

	- Update bundle
		+ gem install bundler

	- install specifc gem version
		+ gem install fog -v 1.8


	- RVM list ruby versions and gemsets
		+ rvm list 
		+ rvm gemset list

	- RVM change ruby and gemset (indivdually and at same time)
	 	+ rvm use 2.3.5
	 	+ rvm gemset use global
	 	+ rvm use 2.3.5@global

	- RVM install ruby and create gemset
		+ rvm install ruby-2.5.3
		+ rvm gemset create blog

	- RVM set default ruby and gemset
		+ rvm --default use 2.5.3
		+ rvm --default use 2.5.3@blog

	- RVM project files to set ruby version and gemset
		+ .ruby-version
		+ .ruby-gemset

	- Rails create a new application
		+ rails new blog
		+ cd blog
		+ bundle install

	- Start web server
		+ rails server (or rails s)

	- Generate a controller
		+ rails generate controller Welcome index 




* Syntax