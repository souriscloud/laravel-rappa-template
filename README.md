#### Docker

* nginx is exposed on :8005

```shell
cp .env.example .env
docker-compose build app
docker-compose up -d
docker-compose exec app composer install
npm i && npm run dev
docker-compose exec app php artisan key:generate
docker-compose exec app php artisan migrate
docker-compose exec app php artisan db:seed
docker-compose exec app php artisan storage:link
```
