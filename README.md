1. docker build -f Dockerfile -t php81container .
2. docker run -v $PWD:/app --rm php81container composer update
3. docker run -v $PWD:/app --rm php81container ./vendor/bin/phpunit tests

or with aliases: php81composer && php81test