# linux_server
Project for Udacity's FSND program in which I secure and set up a Linux server. I also deployed [the catalog project earlier from this degree](https://github.com/kk2385/catalog-app) on this secure web server. This Linux server instance is hosted by Amazon Lightsail.

# Review Info:
IP Address: ```54.210.144.172```
SSH port: ```2200```
URL: http://54.210.144.172

Aside from software obtained from running ```sudo apt-get update``` I also installed the following software on the server:
apache2
libapache2-mod-wsgi
finger
postgresql
python-psycopg2


I also configured ufw with the following:
```
To                         Action      From
--                         ------      ----
2200/tcp                   ALLOW       Anywhere
80/tcp                     ALLOW       Anywhere
123                        ALLOW       Anywhere
2200/tcp (v6)              ALLOW       Anywhere (v6)
80/tcp (v6)                ALLOW       Anywhere (v6)
123 (v6)                   ALLOW       Anywhere (v6)
```

# Resources
I made extensive use of [this tutorial from Digital Ocean on hosting Flask applications on Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps)

