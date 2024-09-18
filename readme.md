# How to run this environmet?

## Here's how to run it !

- Extract this zip if you get this directory in zipped format
- Clone https://github.com/spexf/302_OOP to a file named src, the command will look like this

```
git clone https://github.com/spexf/302_OOP ./src
```

- After cloning the repo, you need to copy this line to an .env file, replace the line that has the same text as text below.

```
DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=laravel
DB_PASSWORD=admin123!
```

- Then, you need to run npm install, you can use this command to run it.

```
docker-compose run --rm -d npm install
```

- just wait till the container stopped.
- if the process is done, then you're ready to run the web app, use this command to run the web app

```
docker-compose up php mysql server npm-run -d
```

- in case there's an error with SQL when you access the web in you browser, run this command

```
docker-compose run artisan migrate
```

- to make a user in filament you can use this command

```
docker-compose run artisan make:filament-user
```

- with the user you create, you can login on the web, just access `http://localhost:9000/admin/login`

### for feedback you can contact me - athkr on discord
