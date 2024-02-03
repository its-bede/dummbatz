# Dummbatz
## A digital version of a card game

* Ruby version --> [.ruby-version](./.ruby-version)
* node version --> [.nvmrc](./.nvmrc)
* System dependencies
    * yarn
    * ruby
    * direnv
    * redis server
    * (docker)

# Configuration
You may want to copy and customize the following `.envrc` and place it into the projects root directory:
```
# .envrc

unset RBENV_VERSION
export EDITOR=vim
export THOR_MERGE=vim
export DOCKER_DEV_DB_PORT=6660
export DOCKER_TEST_DB_PORT=7770
export APP_NAME=dummbatz
```
Make sure to cover at least `DOCKER_DEV_DB_PORT`, `DOCKER_TEST_DB_PORT` and `APP_NAME` in your env config!

# Setup
* Database creation --> run `bin/setup`
* Database initialization --> just run `bin/setup`
* How to run the test suite --> `bin/full-test`
* Run dev environment --> `bin/dev` (If you have NOT installed redis server as a service you need to run `bin/dev -r`)

# Parts
* Services (job queues, cache servers, search engines, etc.)
    * currently none
* Deployment instructions
    * currently none
