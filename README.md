# CommunityGIS

CommunityGIS is a platform for community  for a spatial data infrastructure. 
This consists of frontend described below and backend which is geonode ( see www.geonode.org) 
Primary objective of communitygis is to provide educational platform for learners to learn about spatial information and learn how these modern tools can be used to solve real life problems. As a platform it is for people who range from those who can contribute data ( mobile based point data collection to digitization of published maps) to those who can analyse the data to infer useful social knowledge. It is a digital contraption needed to collect, aggregate , access and analyse data finally provide decision support for to manipulate reality. Since all source code is published hereby (for frontend) , under GPL, any one can reproduce the technology , without any permission from makerGHAT. This has been created by volunteers and coordinated by www.makerghat.org 
This is inspired by ideas as in 'p2p governance' of Bowens ( https://blog.p2pfoundation.net/about ) and Third Pillar of Dr Raghuram Rajan  (https://www.penguinrandomhouse.com/books/566369/the-third-pillar-by-raghuram-rajan/9780525558316/ )

# To run locally, use following guidelines ( you may use makerghat server as backend or install your own )


:boy: You will need python3 and pip3 for installing packages

:baby: fork the repo

:gentleman: clone your repo locally

:grandlady: install postgresql

```
sudo apt-get install postgresql
```
:see_no_evil: create virtual env
```
pip3 -m venv VIRTUALENVNAME 
```
:hear_no_evil: activate virtual env
```
source VIRTUALENVNAME/bin/activate
```
:speak_no_evil: install dependencies
```
python3 install -r requirments.txt
or
python3 install django psycopg2 social-auth-app-django
```
:skull: setup database using [postgres-setup.txt](postgres-setup.txt)

:pray: email at nautiyalanimesh@gmail.com for asking keys for projects

:clap: create tables
```
python3 manage.py migrate
```
:clown_face:create superuser

```
python3 manage.py createsuperuser
```

:tada: run at http://127.0.0.1:8000/
```
python3 manage.py runserver
```
