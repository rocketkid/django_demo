==========
django_demo
==========

This is a Django Demo project based on the book `How to Tango with Django`_

This project is only meant for educational purposes.

The ``dmoz`` and ``mininova`` spiders scrapes the Open Directory Project (dmoz.org) and Mininova Org (mininova.org), and it's based on the examples described in the `Scrapy tutorial`_

``dmoz`` spider doesn't crawl the entire dmoz.org site but only a few pages by
default (defined in the ``start_pages`` attribute). These pages are:

* http://www.dmoz.org/Computers/Programming/Languages/Python/Books/
* http://www.dmoz.org/Computers/Programming/Languages/Python/Resources/


So, if you run the spider regularly (with ``scrapy crawl dmoz``) it will scrape
only those two pages.

If you wish to store the data you can run ``scrapy crawl dmoz -o dmoz_data.json`` and 
it will store the scraped data in a file dmoz_data.json

.. _How to Tango with Django: http://www.tangowithdjango.com/book/index.html

