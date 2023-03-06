# blog-symfony-docker

# Make
```
make help

#symfony racine project
```
docker exec www_blog composer create-project symfony/skeleton:"6.2.*" project
```
composer require webapp
```
docker exec -w /var/www/project www_blog composer req symfony/webpack-encore-bundle
```
docker exec -w /var/www/project www_blog npm install
```
docker exec -w /var/www/project www_blog npm run dev
```
docker exec -w /var/www/project www_blog php bin/console make:controller Home
```

# unlock for dev "install all dependencys and other"
```
sudo chown -R $USER ./




