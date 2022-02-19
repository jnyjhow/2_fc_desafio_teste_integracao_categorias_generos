# start no docker

sudo service docker start
sudo service docker status

# rodando alias

source ~/.bash_aliases

#iniciando com laravel
https://laravel.com/docs/6.x/installation

#criando um novo projeto
composer create-project --prefer-dist laravel/laravel blog "6.*"
cd blog
php artisan serve

# conectando no mysql

docker exec -it micro-videos-db sh
mysql -uroot -proot

docker exec -it micro-videos-app bash

php artisan ide-helper:generate
php artisan ide-helper:models
php artisan ide-helper:meta

#iniciando servidor
php artisan serve

#instalando laravel-ide-helper
composer require --dev barryvdh/laravel-ide-helper

#instalando laravel-dump-server
composer require --dev beyondcode/laravel-dump-server

#verificando comandos do model
php artisan make:model --help

#criando models
php artisan make:model Models/Category --all

#criando seeder
php artisan make:seeder CategoriesTableSeeder

#arrumando a migracao
php artisan migrate:fresh --seed
php artisan migrate:refresh --seed

#verificando dados inseridos
php artisan tinker

#verificando rotas
php artisan route:list

#criando teste unit
php artisan make:test Models/CategoryTest --unit

#criando teste feature
php artisan make:test Models/CategoryTest

#limpando configuracao
php artisan config:cache

#rodando test
vendor/bin/phpunit 

