rendezvous
==========

[![Build Status](https://travis-ci.org/iBenza/rendezvous.png)](https://travis-ci.org/iBenza/rendezvous)
[![Coverage Status](https://coveralls.io/repos/iBenza/rendezvous/badge.png)](https://coveralls.io/r/iBenza/rendezvous)
[![Code Climate](https://codeclimate.com/github/iBenza/rendezvous.png)](https://codeclimate.com/github/iBenza/rendezvous)
[![Dependency Status](https://gemnasium.com/iBenza/rendezvous.png)](https://gemnasium.com/iBenza/rendezvous)

A simple markdown-based blog & wiki system for team.


# Supported versions

- Ruby 2.1.4

# How to install and use.

## Get code and install gems.

```
$ git clone git@github.com:iBenza/rendezvous.git
$ cd rendezvous
$ bundle install
```

## Get Google API Key.

Register application on https://code.google.com/apis/console,
and get

1. Access https://code.google.com/apis/console
2. Create New Project
3. Create Client ID ([APIs & auth] > [Credentials] > [CREATE NEW CLIENT ID])
4. Input form
  - `http://localhost:3000` in [Authorized Javascript origins]
  - `http://localhost:3000/users/auth/google_oauth2/callback` in [Authorized redirect URI]
5. Get [Client ID] and [Client secret]
6. Write your Client ID & Secret in config/settings.yml
7. Input form
  -`rendevous` in [Project name] in Consent screen


## Dotenv


## Setup DB

```
$ (bundle exec) rake db:migrate
$ (bundle exec) rake db:seed
```
And have fun with your team !


# Optional features

## PDF uploading

```
brew install imagemagick ghostscript
```



# Test

Rendezvous uses travis-ci for test.
