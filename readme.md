# Rails 3 Tutorial

## Prolegomenon
Sounds great, Isn't?

##Motivation

This one is easy: I want lo learn Rails.
I will follow the [Ruby on Rails tutorial](http://ruby.railstutorial.org/ruby-on-rails-tutorial-book#top) by Michael Hartl.
I will do it [The hard way](http://ruby.learncodethehardway.org/book/intro.html):
>1. Going throug each exercise.
>2. Typing in sample exactly.
>3. Making it run

## Goals

- Learn Rails
- Improve in:
    -  Ruby
    -  Git
    -  Markdown
    -  …

## My notes

### Chapter 1

##### Setting the mood, tools and environment

Using:

- GIT, git version 1.8.1.1
- Brew, 0.9.3
- Ruby, ruby 1.9.3p327 (2012-11-10 revision 37606) [x86_64-darwin12.2.0]
- RVM, rvm 1.17.0 

-I decided to install Rails using *bundler*.-
Not a good idea, set up is tangled this way.
Installed Rails with 

     $sudo gem install rails


- After running 
    rails new first_app

RVM ask to use the rail's RVM or mine. I kept mine.

- No need to install sqlite-ruby, already in sqlite3 gem.

- Github asking for username and password every push [fixed with](http://stackoverflow.com/questions/7773181/git-keeps-prompting-me-for-password):

>Open .git/config 

>In the [remote "origin"] section
 
    url = ssh://git@github.com/username/repo.gits

- The Gemfile must be modified in order to deploy to Heroku:

    group :development, :test do
      gem 'sqlite3'
    end
    group :production do
     gem 'pg'
    end

Heroku uses Postgres instead of sqlite3.

Now the app lives at [github](https://github.com/rogeliozarate/r3t-firstapp) and runs at [heroku](vhgfckml.herokuapp.com)

### Chapter 2

- I will be working over the previous app. No real need to create a new one.
- I have to pay attention to singular and plural nouns.
- the development records is not migrated to the production database
- After deploying to Heroku it is necessary to migrate the database

### Chapter 3

- It's a time saver to run bundle install without production

       $ bundle install - -without production