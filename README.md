# Use Example

## Create a new project

```
docker run --tty \
           --rm \
	   --volume $PWD/laravel:/var/www/html \
	   shawnoy/laravel \
	   laravel new
```

## Create a special Laravel version

```
docker run --tty \
       --rm \
       --volume $PWD/laravel:/var/www/html \
       shawnoy/laravel \
       composer create-project laravel/laravel ./ 5.2.*
```

## Host a Laravel project

```
docker run --interactive \
           --tty \
	   --volume $PWD/laravel:/var/www/html \
	   --publish 8080:8080 \
	   shawnoy/laravel
```
