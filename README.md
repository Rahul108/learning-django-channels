# Description
This Project is for learning purpose only!

Developed based on the doc of [django-channels](https://channels.readthedocs.io/en/stable/)

Got help from the repo: [YT-Django-Project-Chatroom-Getting-Started](https://github.com/veryacademy/YT-Django-Project-Chatroom-Getting-Started)

# Installation Steps
* Clone this project
```sh
git clone https://github.com/Rahul108/learning-django-channels.git
```

* Create a virtualenv inside the project folder, I've created the virtualenv with python3.8 (my default was 3.9)
```sh
virtualenv .venv --python=python38
```

* Install those following packages
```sh
pip install django
pip install channels
pip install channels_redis
```

* Install Redis (followed the [official doc](https://redis.io/topics/quickstart))
```sh
# Install if not installed previously
wget http://download.redis.io/redis-stable.tar.gz
tar xvzf redis-stable.tar.gz
cd redis-stable
make
sudo make install

# Run Redis Server
redis-server
```

* Migrate DB
```sh
python manage.py migrate
```

* Create a Super-User
```sh
python manage.py createsuperuser
```

* Run the project
```sh
python manage.py runserver
```


* Browse the project on
```sh
localhost:8000/

# For Chatbox
localhost:8000/chat/

# Open Specific ChatGroup
localhost:8000/chat/<chatgroup>/  # e.g  localhost:8000/chat/g1/
```