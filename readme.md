# Laravel Framework 5.1  Bootstrap 3 Starter Site

Demo site is deleteed today> It's because some user upload virus code which is stop work server, which I use to hosting, and I need do delete it. Host owner tell me that I have some virus code on my start site(someone is upload some virus code on server) and I need to delete it or they delete it. So I must delete it. Sorry.

## Starter Site based on on Laravel 5.1 and Boostrap 3
* [Features](#feature1)
* [Requirements](#feature2)
* [How to install](#feature3)
* [Application Structure](#feature4)
* [Troubleshooting](#feature5)
* [License](#feature6)
* [Additional information](#feature7)
* [How Starter site is look like](#feature8)
* [Advanced Alternatives](#feature9)

<a name="feature1"></a>
## Starter Site Features:
* Laravel 5.1.x
* Twitter Bootstrap 3.x
* Back-end
	* Automatic install and setup website.
	* User management.
	* Manage languages.
	* Manage photos and photo albums.
	* Manage article and article categories.
    * DataTables dynamic table sorting and filtering.
    * Colorbox jQuery modal popup.
    * Add Summernote WYSIWYG in textareas.
* Front-end
	* User login, registration
	* View Photos,Articles, Languages and Users
	* soon will be more...
* Packages included:
	* Datatables Bundle

-----
<a name="feature2"></a>
##Requirements

Make sure all the required PHP extensions are loaded in your php.ini file.

	PHP >= 5.5.9
	OpenSSL PHP Extension
	Mbstring PHP Extension
	Tokenizer PHP Extension
	Fileinfo PHP extension
	SQL server(for example MySQL)
	Composer
	Node JS

-----
<a name="feature3"></a>
##How to install:
* [Step 1: Download the repository](#step1)
* [Step 2: Use Composer to install PHP dependencies](#step2)
* [Step 3: Create database, set up .env file, run migrations and seeds](#step3)
* [Step 4: Install node.js, bower, gulp and compile assets](#step4)
* [Step 5: Start Page](#step5)

-----
<a name="step1"></a>
### Step 1: Download the repository

Create new project folder and change directory into it.

You also can create new vhost on your HTTP server (for example Apache's <vhost>) and add your local host to system `hosts` file, for example, to make your site accessible via http://mywebsite.local. Make sure DocumentRoot is set to project_folder/public.

There are two ways to download Laravel-5-Bootstrap-3-Starter-Site: using git or downloading zip archive.

Download the git repository

    git clone https://github.com/mrakodol/Laravel-5-Bootstrap-3-Starter-Site.git .
    
If you have your own remote git repository, change origin url.

    git remote set-url origin https://HOST.COM/OTHERREPOSITORY.git
    
If you don't have remote git repository, remove origin:

    git remote rm origin

OR without using git you can download zip archive and extract it into project folder.

    https://github.com/mrakodol/Laravel-5-Bootstrap-3-Starter-Site/archive/master.zip


-----
<a name="step2"></a>
### Step 2: Use Composer to install PHP dependencies

Laravel utilizes [Composer](http://getcomposer.org/) to manage its dependencies. First, download a copy of the composer.phar.
Once you have the PHAR archive, you can either keep it in your local project directory or move to
usr/local/bin to use it globally on your system.
On Windows, you can use the Composer [Windows installer](https://getcomposer.org/Composer-Setup.exe).

To install all the PHP dependencies run:

    composer install


-----
<a name="step3"></a>
### Step 3: Create database, set up .env file, run migrations and seeds

Create new database with utf-8 collation (`uft8_general_ci`) on your MySQL database server. You can create additional user and password.

After that, copy `.env.example` and rename it as `.env` and put your MySQL server and database credentials, change default database host name, database name, username and password.

Now that you have the environment configured, you need to run Laravel migrations to create all the tables:

    php artisan migrate

(Optional) To initial populate database use this:

    php artisan db:seed


-----
<a name="step4"></a>
### Step 4: Install node.js, bower, gulp and compile assets

This project makes use of Bower and Laravel Elixir. Before triggering Elixir, you must first ensure that Node.js (included in homestead) is installed on your machine.

    node -v

Install dependencies listed in package.json with:

    npm install

If you don't have Bower installed globally:

    npm install -g bower

Retrieve frontend dependencies from bower.json with Bower:

    bower install

Using gulp and Laravel elixir compile SASS, merge CSS, JS and move frontend files (images, fonts, etc) into public directory:

    gulp

or to also minify all the assets for better perfomance:

    gulp --production


-----
<a name="step5"></a>
### Step 5: Start Page

You can now login to admin part of Laravel Framework 5  Bootstrap 3 Starter Site:

    username: admin@admin.com
    password: admin
OR user

    username: user@user.com
    password: user

-----
<a name="feature5"></a>
## Troubleshooting

### RuntimeException : No supported encrypter found. The cipher and / or key length are invalid.

    php artisan key:generate

### Site loading very slow

	composer dump-autoload --optimize
OR

    php artisan dump-autoload

-----
<a name="feature6"></a>
## License

This is free software distributed under the terms of the MIT license

-----
<a name="feature7"></a>
## Additional information

Inspired by and based on [andrew13's Laravel-4-Bootstrap-Starter-Site](https://github.com/andrew13/Laravel-4-Bootstrap-Starter-Site)

----
<a name="feature8"></a>
##How Starter Site is look like

![Index](http://i57.tinypic.com/2yug28x.jpg)
![Login](http://i58.tinypic.com/r7p4et.jpg)
![Register new user](http://i61.tinypic.com/fvcz5x.jpg)
![Admin dashboard](http://i58.tinypic.com/b9g2g1.jpg)
![Admin users](http://i60.tinypic.com/301hemp.jpg)
![Admin list users](http://i58.tinypic.com/2ujl5dh.jpg)

----
<a name="feature9"></a>
## Advanced alternatives
If you are interested in advanced starter sites where you can get 70+ admin pages, 20+ frontend pages with color schemes and a CRUD generator then visit below links

[Josh](http://goo.gl/Mnhunr)

[Chandra](http://goo.gl/hk4ut3)
