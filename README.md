# learnscrapy
learning scrapy for webscraping

create a new directory and a virtual environment for our project

    $ mkdir project01; cd project01
    $ python3 -m venv venv
    $ source venv/bin/activate

Now our environment is ready, we can install the following python libraries with pip package manager.

    $ pip install --upgrade pip
    $ pip install scrapy psycopg

To start a scapy project run

    $ scrapy startproject <project_name>

To generate our scrapy spider let's run;

    $ scrapy genspider <spider-name> <url-to-scrape>
    
To open a scrapy shell use command

    $ scrapy shell

To fetch within the shell

    $ fetch('url-to-scrape')

To run our scrapy spider

    $ scrapy crawl <spider-name>
    $ scrapy crawl <spider-name> -O filename.json

To run an already defined spider project, navigate to where the spider file is located or include its path in the following command:

    $ scrapy runspider /path/to/spiders/spider-file.py

If you have this repository cloned run:

    $ scrapy runspider learnscrapy/bookscraper/spiders/bookspider.py

**note it's important to understand css and html for successfull scraping**

**HAPPY WEB SCRAPING**
