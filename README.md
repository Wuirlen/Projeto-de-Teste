### 1. Usando Docker
Caso não utilize Docker, faça o `git clone` no ambiente desejado e ignore os comandos `docker-compose`.
```
~$ git clone <projeto git>
~$ docker-compose up -d

//Docker bash ou qualquer que seja o ambiente que esteja rodando.
~$bash composer update


//Copie e altere o arquivo .env
~$bash cp .env.example .env
~$bash vim .env

DB_CONNECTION=mysql
DB_HOST=192.168.0.4
DB_PORT=3306
DB_DATABASE=mindtec
DB_USERNAME=root
DB_PASSWORD=root

~$bash php artisan key:generate
~$bash php artisan migrate
~$bash php artisan migrate --seed


```