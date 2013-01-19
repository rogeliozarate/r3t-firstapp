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

I decided to install Rails using *bundler*

- After running 
    rails new first_app

RVM ask to use the rail's RVM or mine. I kept mine.

- I had to install 'sqlite2-ruby' gem, specific for OS X.
- Github asking for username and password every push [fixed with](http://stackoverflow.com/questions/7773181/git-keeps-prompting-me-for-password):

>1. Open .git/config 
>2. In the [remote "origin"] section 
>>     set url = ssh://git@github.com/username/repo.gits

