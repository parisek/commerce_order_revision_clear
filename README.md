Commerce order revision clear
===

This is lightweight module that solves issue that database is getting really huge because we are storing all revisions for commerce orders. In our commerce site we have orders with hundreds of revisions.

How it works?
===
We are using [https://www.drupal.org/project/commerce/issues/2442049](https://www.drupal.org/project/commerce/issues/2442049) code from provided batch to leverage Entity API module. With every CRON run we delete 50 oldest revisions which are older than 30 days. This module has no configuration, but could be easily customized in code for your special needs.

**Do not test in production and backup your database**

Author
===
Petr Parimucha

[https://pari.cz](https://pari.cz/en)
