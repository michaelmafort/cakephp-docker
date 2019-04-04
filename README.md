# CakePHP Docker Environment

A minimalist docker setup to create your first CakePHP application.

The framework source code can be found here: [cakephp/cakephp](https://github.com/cakephp/cakephp).

## Installation

To run this environment you need the [PHP Composer](https://getcomposer.org/doc/00-intro.md) and [Docker Desktop](https://www.docker.com/products/docker-desktop) installed.
1. Clone this Repo `git clone git@github.com:michaelmafort/cakephp-docker.git`
2. Change the directory to cakephp-docker, `cd ./cakephp-docker`
3. Install [Composer](https://getcomposer.org/doc/00-intro.md) on binary folder or update `composer self-update`
4. Run `composer create-project --prefer-dist cakephp/app app`
5. Install [Docker Desktop](https://www.docker.com/products/docker-desktop)
6. Install [Docker Compose](https://docs.docker.com/compose/install/)
7. Start the docker services `docker-compose up`
8. Wait to services up and then visit `http://localhost:8080` to see the welcome page.
9. Change `app/config/app.php` MySQL configuration to:
```bash
'host' => 'cakephp-mysql',
'username' => 'root',
'password' => 'root',
'database' => 'cakephp'
```