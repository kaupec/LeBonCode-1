# Le Bon Code Julien Le Touzic

## Requirements
- php 8.1
- docker
- docker-compose

## Installation

`docker-compose up -d`

`composer install`

`php bin/console lexik:jwt:generate-keypair`

`php bin/console doctrine:database:create`

`php bin/console doctrine:migrations:migrate`

`symfony server:start`

## How to use API

Go to http://127.0.0.1:8000/api

Create a user

Login with the user and get a token

Click on the authorize green button and enter `Bearer YOUR_TOKEN`

Now you can use API

## Area of improvements

- Adding end-to-end testing with fixtures
- Build a complete environment with docker and a makefile
- Better price management with a data transformer for example
- Separate entities and API resources with custom data persisters and data providers to be more ddd.
- Put an all ddd design pattern with command bus symfony and be more doctrine agnostic.

