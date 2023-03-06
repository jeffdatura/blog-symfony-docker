# blog-symfony-docker

# Make
```
make help
```

#symfony racine project
```
docker exec www_blog composer create-project symfony/skeleton:"6.2.*" project
```
```
cd project
```
```
composer require webapp
```
```
docker exec -w /var/www/project www_blog composer req symfony/webpack-encore-bundle
```
```
docker exec -w /var/www/project www_blog npm install
```
```
docker exec -w /var/www/project www_blog npm run dev
```
```
docker exec -w /var/www/project www_blog symfony console make:controller Home
```
```
docker exec -w /var/www/project www_blog symfony local:php:list
```
```
DATABASE_URL="mysql://root:@db_blog:3306/symfony?serverVersion=8&charset=utf8mb4"
```
```
make database-create

# unlock for dev "install all dependencies and other"
```
sudo chown -R $USER ./
```



