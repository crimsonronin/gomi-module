Zoop gomi-module
================

[![Build Status](https://api.shippable.com/projects/53f6a51bec49367903313063/badge/master)](https://www.shippable.com/projects/53f6a51bec49367903313063)

Provides a simple user module for use in <a href="http://zoopcommerce.github.io/shard-module">shard-module</a>.

Also provides a REST interface for users to change and recover passwords.

Install
-------

Add the following to your composer root:

    "require": {
        "zoopcommerce/gomi-module" : "~1.0"
    }

Add the module to your application config:

    'modules' => [
        'Zoop\GomiModule'
    ],

Configuration
-------------

See `config/module.config.php` comments for configuration options.

_Note_ Do not neglect to change the email salt and encryption key.

Use
---

To begin password recovery go to:

    /rest/recoverpassword/token

To complete the password recovery, follow the link in the sent email.
