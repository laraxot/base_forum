## Starting project of a classic forum, currently to be implemented

## Installation instructions

```
git clone https://github.com/laraxot/base_forum.git forum --recurse-submodules --depth 1
```
or
Create a new folder in your workspace
```
mkdir forum
cd forum
```
Via git bash executed
```
git init
```
Continue with
```
git remote add origin https://github.com/laraxot/base_forum.git
git pull origin master
git submodule update --init --checkout --force
```
In the project [forum] folder
```
cd laravel
```
create the .env file of your project
```
cp .env.latest .env
```
Set the database using these 2 lines
```
DB_DATABASE=geek_forum
DB_DATABASE_LU=geek_lu
```
Run
```
composer update
```
Create the app_key
```
php artisan key:generate
```
run the migration to create the database
```
php artisan migrate
```

Enjoy ;)
