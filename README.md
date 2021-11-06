apt update 
apt upgrade
apt install git
apt install python3 
apt install python3-pip
pip3 install django==2.1.1
pip3 install chatterbot==0.8.7
pip3 install chatterbot-corpus==1.1.2
django-admin startproject cb
cd cb/cb
nano settings.py                                            #ifconfig (allowed host['IP'])    #install apps['sili']
nano urls.py                                                #add=from django.conf.urls import include path.add=path('',include('sili.urls'))
cd ..
git clone https://github.com/NeelimaBalaji/sili
python3 manage.py migrate
python3 manage.py runserver 0.0.0.0:8000
