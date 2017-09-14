# CodeIgniter Command Line Worker

Works in a similar way to that of Laravel's Artisan command line tool - you can create controllers, models and libraries at the moment in this very early stage.

I'll be adding a lot more to this script at a later date:
- Migrations
- Seeders
- Database interaction (both using existing models and direct input)
- Along with additions to the controllers/models/libraries creators

#### Installation
```sh
$ cd your/codeigniter/project
$ git clone https://github.com/richardhedges/CodeIgniter-Worker.git
```

#### Example usage
Start the webserver:
```sh
$ php worker serve
```
Creating a controller:
```sh
$ php worker make:controller Welcome
```
Creating a model:
```sh
$ php worker make:model Users
```
Creating a model (and define the table):
```sh
$ php worker make:model Forum --table forum_posts
```
Creating a library:
```sh
$ php worker make:library Template
```
Creating a view:
```sh
$ php worker make:view login
```

#### Requirements
The models created with worker extend a core model `MY_Model.php`. This is because of the extra functionality I plan to add at a later date - the `MY_Model.php` file has been included in this repo (credits to its creator are included in the file).