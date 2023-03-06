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

# unlock for dev "install all dependencies and other"
```
sudo chown -R $USER ./
```



