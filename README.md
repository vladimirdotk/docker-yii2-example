Yii2 + Docker example
==================================
> Includes nginx, php-fpm, mysql and redis. Generated by https://phpdocker.io/generator
## How To start
+ Run docker-compose `docker-compose up -d`
+ Install composer-asset-plugin `docker exec -it docker-yii2-example-php-fpm composer global require "fxp/composer-asset-plugin:^1.3.1"`
+ Install yii2 basic app `docker exec -it docker-yii2-example-php-fpm composer create-project --prefer-dist yiisoft/yii2-app-basic app` (will require github token)
+ Install yii2-redis extension `docker exec -it docker-yii2-example-php-fpm composer -d=app require --prefer-dist yiisoft/yii2-redis`
+ Own generated files `sudo chown $USER:$USER -R app`
+ Go to http://localhost:8080 to see Yii start page
+ Change docker-compose.yml and related files to fit your needs
