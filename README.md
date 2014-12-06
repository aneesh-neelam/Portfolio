Portfolio
=========

The code repository for my Portfolio Website

The website is hosted [here](http://aneeshneelam.me/)

Please report any bugs or issues [here](https://github.com/aneesh-neelam/Portfolio/issues)

#### Instructions for Installation:
###### Create a Python 3.4.x Virtualenv and activate it
###### Install Python project dependencies

    $ pip install -r requirements.txt

###### Install Node.js 0.10.x and Bower
###### Install Bower components

    # npm install -g bower
    $ bower install
    
###### Django Tasks
    
    $ python manage.py migrate
    $ python manage.py collectstatic
    
###### Run the server locally at port "$PORT" in os.environ or a manually entered port

    $ python manage.py runserver $PORT (For Development)
    $ waitress-serve --port=$PORT portfolio.wsgi:application (For Production)
    
#### External Requirements:
* A PostgreSQL instance running locally or valid "DATABASE_URL" string in os.environ
* A valid "SECRET_KEY" string in os.environ for better security (Optional)

#### Custom buildpack for Heroku
* Set BUILDPACK_URL in os.environ as [this](https://github.com/papaeye/heroku-buildpack-python-bower.git)
