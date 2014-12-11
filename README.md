grasshopper
===========

# Build status
[![Build Status](https://travis-ci.org/fronteerio/grasshopper.png?branch=master)](https://travis-ci.org/fronteerio/grasshopper)
[![Coverage Status](https://coveralls.io/repos/fronteerio/grasshopper/badge.png)](https://coveralls.io/r/fronteerio/grasshopper)

Grasshopper Event Engine

# Build status
[![Build Status](https://travis-ci.org/CUL-DigitalServices/grasshopper.svg?branch=master)](https://travis-ci.org/CUL-DigitalServices/grasshopper)

# Setup

This documentation assumes you're running OS X with homebrew.


##  Postgres
```
# Install postgres
brew install postgresql

# Start postgres
postgres -D /usr/local/var/postgres

# Create a database and user
psql template1
    template1=# CREATE USER grasshopper WITH PASSWORD 'grasshopper';
        CREATE ROLE
    template1=# CREATE DATABASE grasshopper;
        CREATE DATABASE
    template1=# CREATE DATABASE grasshoppertest;
        CREATE DATABASE
    template1=# GRANT ALL PRIVILEGES ON DATABASE grasshopper TO grasshopper;
        GRANT
    template1=# GRANT ALL PRIVILEGES ON DATABASE grasshoppertest TO grasshopper;
        GRANT
```


## Grasshopper
```
# Clone the application somewhere
git clone git://github.com/fronteerio/grasshopper

# Install the npm dependencies
npm install

# Install the grunt CLI (globally)
npm install -g grunt-cli

# Run the application
node app
```
