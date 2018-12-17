# Use Example

## Create a new project

```
docker run --tty \
           --rm \
	   --volume $PWD/laravel:/var/www/html \
	   laravel \
	   laravel new
```

## Host a Laravel project

```
docker run --interactive \
           --tty \
	   --volume $PWD/laravel:/var/www/html \
	   --publish 8080:8080 \
	   laravel
```