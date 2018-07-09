# Super Blog Dependencies

Make sure you are able to run the server and system tests prior to our pairing session.


### Setup

* Install ruby 2.5.1.  If using [rbenv](https://github.com/rbenv/rbenv) then `rbenv install 2.5.1`
* Install [bundler](https://bundler.io/). `gem install bundler`
* Install dependencies for this application: `bundle install`
* Install Google Chrome which is used in the system tests


### Run Local Server

Create database and load demo data...
```
bundle exec rake db:drop db:create db:migrate db:setup
```

Run server and access it on localhost:3000

```
bundle exec rails s
```


### Tests

Run model tests...
```
bundle exec rails test
```

Run System tests...
```
bundle exec rails test:system
```

Lint...
```
bundle exec rubocop
```


# Agenda

1) I'll give you a brief introduction to the codebase

2) We will work together to fix all the tests

3) Open up BUGS.md.  We'll discuss how to attack these and if there's enough time implement fixes.

4) Open up TODO.md.  We'll note what could be improved in this app.
