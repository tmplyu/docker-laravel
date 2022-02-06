# docker-laravel

### VB 起動

```
vagrant up
vagrant ssh
```

### docker 起動

```
cd project
docker-compose up -d
```

### Laravel install

```
docker-compose exec php composer create-project laravel/laravel --prefer-dist . "8.x"
docker-compose exec php php artisan storage:link
docker-compose exec php chmod -R 777 storage
```