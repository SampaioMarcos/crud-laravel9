
# Aplicação web utilizando framework laravel 9 para fins didáticos utilizando:

* PHP 
* CSS
* MYSQL
* LARAVEL 
* ELOQUENT
* BOOTSTRAP
* RESTFUL
* MIDDLEWARE
* DOCKER

### RELACIONAMENTOS
* User (1:N) Post
* User (1:N) Comment
## Autenticação Laravel Breeze!
![tela-login](https://user-images.githubusercontent.com/46831962/191051598-875dee3f-606f-4e9f-8b44-b3ccfa035b43.png)

## Formulário para cadastrar Post!
![tela-cadastrar-post](https://user-images.githubusercontent.com/46831962/191047833-70c4c2c3-e17e-4764-9160-672b67fd2359.png)
## Post Listados!
![pagina-posts-listados-](https://user-images.githubusercontent.com/46831962/191048985-e0eb26bd-998d-4799-afb8-edc7a97d36c2.png)
## Página de Detalhes!
![tela-detalhaes](https://user-images.githubusercontent.com/46831962/191049426-ec995823-5ef5-4450-b6fa-6cfd485621d7.png)

## Validação de campos do formulário de cadastro e atualização!
![validaça](https://user-images.githubusercontent.com/46831962/191049707-cda632c2-32bd-4d55-aac4-79b06029921b.png)


# Setup Docker Para Projetos Laravel 9 com PHP 8

### Passo a passo
Clone Repositório
```sh
git clone https://github.com/especializati/setup-docker-laravel.git laravel9
```

```sh
cd laravel9/
```


Alterne para a branch laravel 8.x
```sh
git checkout laravel-9-com-php-8
```


Remova o versionamento
```sh
rm -rf .git/
```


Crie o Arquivo .env
```sh
cd example-project/
cp .env.example .env
```


Atualize as variáveis de ambiente do arquivo .env
```dosini
APP_URL=http://localhost:8989

DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=nome_que_desejar_db
DB_USERNAME=root
DB_PASSWORD=root

CACHE_DRIVER=redis
QUEUE_CONNECTION=redis
SESSION_DRIVER=redis

REDIS_HOST=redis
REDIS_PASSWORD=null
REDIS_PORT=6379
```


Suba os containers do projeto
```sh
docker-compose up -d
```


Acessar o container
```sh
docker-compose exec app bash
```


Instalar as dependências do projeto
```sh
composer install
```


Gerar a key do projeto Laravel
```sh
php artisan key:generate
```


Acesse o projeto
[http://localhost:8989](http://localhost:8989)
