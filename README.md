# CodeIgniter Command Line Worker

A command line tool to help create controllers, models, libraries and more.

#### Requirements
The models created with worker extend a core model `MY_Model.php`. The `MY_Model.php` file has been included in this repo (credits to its creator are included in the file).

The playground needs [psysh](http://psysh.org/) to work at all, installation instructions provided (documentation available on their website).

#### Installation
```sh
$ cd your/codeigniter/project
$ git clone https://github.com/richardhedges/CodeIgniter-Worker.git
$ composer require psy/psysh:@stable
```

#### Example usage
Start the webserver:
```sh
$ php worker serve
```
Run the playground:
```sh
$ php worker playground
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
