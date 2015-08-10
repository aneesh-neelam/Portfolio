Portfolio
=========

This is the code repository for my Portfolio Website

The website is hosted [here](http://aneeshneelam.me/)

Please report any bugs or issues [here](https://github.com/aneesh-neelam/Portfolio/issues)

#### Instructions for Installation:
###### Install all dependencies

    $ pip install -r requirements.txt
    $ bower install

###### Django Tasks

    $ python manage.py migrate
    $ python manage.py collectstatic

###### Run the server locally at port "$PORT" in os.environ or a manually entered port

    $ python manage.py runserver $PORT (For Development)
    $ gunicorn portfolio.wsgi --log-file - (For Production)

#### External Requirements:
* PostgreSQL
