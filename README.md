# User-module
This is a laravel-module that extracts basic user authentication logic and ui from laravel 6. 

A laravel-module is a kind of composer module created for module management 
[Laravel Module](https://github.com/nWidart/laravel-modules)

## Background
Adding user authentication to laravel is easy and straight forward, just follow the 
[instructions](https://laravel.com/docs/5.7/authentication) from laravel website. 
But it still a process developer has to repeat for every website, and it applies to the root code base and not modular.

Laravel-module is a good way to organize the code and make it easy to share and extend the functions. Making the basic
user authentication as a laravel-module makes it easier to add user support. It is also easy to switch between
different user management module.

## Usage

 ```shell
laravel new blog
cd blog
composer require laravel/ui
composer require nwidart/laravel-modules
composer dump-autoload
artisan ui bootstrap
composer require tongdu99/user-module
npm install && npm run dev
artisan migrate
 ```

Now when you visit [blog.test](http://blog.test), you will see the Login and Register menu item on the top right corner. 
