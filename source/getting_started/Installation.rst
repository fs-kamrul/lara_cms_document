
Installation
############

Introduction
============

:ref:`#Requirement <hwRequirement>`

:ref:`#Installation <hwInstallation>`

:ref:`#Install on Hosting <hwInstallHosting>`

:ref:`#Install locally or in VPS <hwLocallyVPS>`

.. _hwRequirement:

Requirement
===========

* Apache, nginx, or another compatible web server.
* PHP >= 8.0 >> Higher
* MySQL Database server
* BCMath PHP Extension
* Ctype PHP Extension
* Fileinfo PHP extension
* JSON PHP Extension
* Mbstring PHP Extension
* OpenSSL PHP Extension
* PDO PHP Extension
* Tokenizer PHP Extension
* XML PHP Extension
* Module Re_write server
* PHP_CURL Module Enable

.. _hwInstallation:

PHP Configuration
=================

Open your php configuration file php.ini and change the following settings.


.. code-block:: php
   :linenos:

    memory_limit = 64M
    max_execution_time = 300

If you are using Cpanel, you can follow this article to change your PHP memory limit settings
https://chemicloud.com/kb/article/how-to-increase-the-php-memory-limit-in-cpanel/

`Laravel documentation page <https://www.laravel.com/docs/>`

.. note::
   On this project, we're using the latest Laravel version (currently 8.x).
   Please go to `Laravel documentation page <https://www.laravel.com/docs/>` for more information.

   It’s based on Laravel framework, the root folder for it is /public.
   You shouldn’t install it on a sub-folder, use sub-domain is better than sub-folder. (we won’t support to install our product on sub-folder).

.. _hwInstallHosting:

Install on hosting
==================

.. note::
   If you're a Laravel developer and you want to customize our source code
   in ``Module`` and ``themes``, you need to delete folder /vendor then
   run command ``composer install`` to reinstall vendor packages.

* Upload all files into the root folder of your hosting (normally, it is ``public_html``).
* Create a database and import data from ``database.sql`` (it's located in source code). Database
* Update your database credentials and ``APP_URL`` in ``.env``

.. image:: /images/database.png

* Go to /admin to access to admin panel.
* The default admin account is ``kamrul@gmail.com`` - ``12345678``.

.. _hwLocallyVPS:

Install locally or in VPS
=========================

.. note::
   If you're a Laravel developer and you want to customize our source code
   in ``Module`` and ``themes``, you need to delete folder /vendor then
   run command ``composer install`` to reinstall vendor packages.

* Update your database credentials and APP_URL in ``.env``

.. image:: /images/database.png

* Using sample data:
* Import database from database.sql.
* Don't use sample data:
   * Run ``php artisan migrate`` to create database structure.
   * Run ``php artisan kamul:user:create`` to create admin user.
   * Run ``php artisan kamul:theme:activate`` stories
* If you're pulled source code from GIT server:
   * Run ``php artisan vendor:publish --tag=kamuldashboard_public --force``
   * Run ``php artisan kamul:theme:assets:publish``
* Run web locally:
   * Change ``APP_URL`` in .env to ``APP_URL=http://localhost:8000``
   * Run ``php artisan serve``. Open `http://localhost:8000``, you should see the homepage.
   * Go to ``/login`` to access to admin panel.
   * If you're using sample data, the default admin account is ``kamrul@gmail.com`` - ``12345678``.
   * If you don't use sample data, you need to go to -> Plugins then activate all plugins.
