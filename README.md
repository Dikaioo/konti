# konti

Contributions tracking...

```sh
$ git clone git@github.com:geekquest/konti.git

$ cd konti
```

## First time setup with Docker

```sh
$ docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v "$(pwd):/var/www/html" \
    -w /var/www/html \
    laravelsail/php82-composer:latest \
    composer install --ignore-platform-reqs
```

Then with sail

```sh
$ ./vendor/bin/sail up
```

Not using sail? You should be able to get around with composer and your regular Laravel commands...
