Django Querycount
=================

.. image:: screenshot.png
    :alt: django-querycount in action

Inspired by `this post by David Szotten <http://goo.gl/UUKN0r>`_, this project
gives you a middleware that prints DB query counts in Django's runserver
console output.


Installation
------------

    pip install django-querycount

Just add ``querycount.middleware.QueryCountMiddleware`` to your ``MIDDLEWARE_CLASSES``.

Notice that django-querycount is hard coded to work only in DEBUG mode set to true

Settings
--------
set QUERYCOUNT_THRESHOLDS in your settings file to your preference
defaults to: {'MEDIUM': 50, 'HIGH': 200, 'MIN_TIME_TO_LOG':0, 'MIN_QUERY_COUNT_TO_LOG':0}


License
-------

This code is distributed under the terms of the MIT license.

Testing
-------

Works only in context of a django installation venv: cd querycount/tests && python test.py 
