Catalog Project (Hiking Days with Friends):

URL: http://www.hikingdayswithfriends.com/ (Public IP:54.186.231.81)
 Note: you can login with google account, however, facebook accout is not working because facebook doesn't allow a transaction with http.

Github (default): https://github.com/nob496/catalog

SSH access for ubuntu
 sudo ssh ubuntu@54.186.231.81 -p 2200 -i ~~~~~.pem

SSH access for grader
 sudo ssh grader@54.186.231.81 -p 2200 -i id_rsa

id_rsa (private key):
-----BEGIN RSA PRIVATE KEY-----
MIIEowIBAAKCAQEAs29wpJekYq5Mi5Z++k40gIl7PeLIq4D8DiyJC6CENyxWmmT/
C0swALkRu5FJ3Q6lGBokocyMQenWEpSxKXYM2TDvk7+vQRVZKkcK7XgSd0I2wEhR
XGW5eXICcwuOonF55mmLKRCcu0OuqrAf4NfsJcXerbLZbUAvR7iQdDR2sbRdOEGJ
1WLdMchxkKgxon9A1gAAXOmtzcBqtu99dmyTvO6iJF075x1fkbCRJKg/M4f8ivgX
+JxrPnewub69YXdzvul0/yLaIj5RP1Dokok63exJYVgTXVRi0PB+illcLXO1xlje
BTpSfB13K0rJvAmV4vKzyjkWdUu30kDWYR88+QIDAQABAoIBAEp7g8KOv8nGmDeJ
LQQx2lFQwDucG7g1PmuTyP9ujfNpEDnemo/Rkgd6ywWU9ZgxMA6lK3eONNpXemkU
F8YiHos5aPlnpBPcDLsj6kFQijm+3oNKgZtdDnR/As1GitqbSAKA5ScSojyJh8OK
gHEQsBGt5RUtHFvhPL8EudHCxVJV3iZPAeoKf4OhNZgoso8U/abk9OrcyHHnPu3e
zEvy1uvouqnf6xhXIV6ejBbpH02Vvra2bhNvkhw7CdpF28t810+VTfEG0ziJpAC9
35YFs+yIoOtY5/fPdsGna2S61Br51K2ehF9VEK+dKsjp/lHIve2WAW1wdPe3usSX
AxzC6gECgYEA3T7xKq2eCzuOCB++iC6seNgnD14AntIgrT0WWO9XwdHdodNXuTIs
X7ojGo9y/XWbfV8t6t3uaZHJ/2F1mCfwy35M8Z101iNVIhnM2yA2o5uBFhaDweIg
m2KNWJ9dD737tZcjOLuPy8LSbZni71qm7r0aidXoREvJlPtihHFXQJECgYEAz58m
0Dh6UB2+tdcpxwpubAjQb6lCifhaIhTNVyrUgFK8BSXSiOpLz/INkciwsz5FhCKr
dAp6dfN4rIOwag7yjJT10ntrWaLehsqOZp7Ngn931ZCsw3P6/dAL7D/r6qnVIQz2
nXDgA8M2ia4ea/E48uX3pDggxIjFwSgVBBiaaekCgYBAMU356wvrCGmKU+ONUbV7
DoQuwkB91Evk18+PGEqnEsQyesZ+Fl+nmrMqtqpPffsSYjZJagENol4wec+LyTLl
aAzdIalPpErELSYyAeO4jprilL+/1mNNkkeeigaPVbkdk++FO25aWXmCkV61weCj
bjyv919/yVmAn3uTH+uH8QKBgAmERgctT430jxVOs3+IHt+c19EGdSJV2+vMAE2K
jQsEv9GMlkXoV2lEsxKHnHHa3NzdqfY7tLlLW7CsqJ1z6fI/sbTgK1+Ec6bCChzy
EoF0zk1fwEuFOXAA5UsC8xFij35gVb2JuvrxK8LL1GEmQXIA0IUafYYEruvXpn71
kb5hAoGBAI6A1VoGX45+Ghx5CHGGX/h/+TURNJ3C/XodoJ7tkXBoTJjCzrvfnvyR
XwXbqMqR3wcIcSg+6CPaD+6W7I+4T+WOcGIhcn1QgoGGLylkpjzYQiUelO2a4vPX
JXt4iSMa/GyL0wHyKYfmvlnWrboi63Mfg9Fqm7RQ9+3rfaormqzd
-----END RSA PRIVATE KEY-----

Softwares installed
 -apache2 (https://httpd.apache.org/): Apache HTTP Server
 -libapache2-mod-wsgi (http://flask.pocoo.org/docs/1.0/deploying/mod_wsgi/): The mod_wsgi package implements a simple to use Apache module which can host any Python web application which supports the Python WSGI specification.
 -python-setuptools: https://setuptools.readthedocs.io/en/latest/
 -postgresql(https://www.postgresql.org/): open source object-relational database system.
 -git: to clone my remote repository (https://github.com/nob496/catalog)
 -python-psycopg2 (http://initd.org/psycopg/): Psycopg is the most popular PostgreSQL adapter for the Python programming language.
 -python: ver.2.7.12
 -python-pip: python package management

Python packages
 -flask (http://flask.pocoo.org/): API to create Web app with Python script.
 -sqlalchemy (https://www.sqlalchemy.org/): python SQL toolkit and Object Relational Mapper.
 -oauth2client (https://oauth2client.readthedocs.io/en/latest/): makes it easy to interact with OAuth2-protected resources.
 -requests (https://2.python-requests.org//en/master/): the only Non-GMO HTTP library for Python.

APP (directory strucure)
/var/www/catalog
            |-----/catalog.wsgi
            |-----/catalog
                      |-----/__init__.py
                      |-----/database_setup.py
                      |-----/hikingtrails.py
                      |-----/client_secrets.json
                      |-----/fb_client_secrets.json
                      |-----/static
                               |-----/style.css
                      |-----/templates
                               |-----/hikingDays.html
                               |-----/trailInfo.html
                               |-----/header.html
                               |-----/login.html
                               |-----/editPark.html
                               |-----/deletePark.html
                               |-----/editTrailInfo.html
                               |-----/deleteTrail.html
                               |-----/newPark.html
                               |-----/newTrailInfo.html

Files Created for Configuration
 /var/www/catalog/catalog.wsgi
 /etc/apache2/sites-available/catalog.conf

Error Log
 sudo/var/log/apache2/error.log (with cat or  tail -f)

Procedure:
1. AWS Lightsail (Ubuntu 16.04 OS only)
   Instance Name: hiking-app-nob496-1

2. Initial setting
  (1) sudo apt-get update
  (2) sudo apt-get upgrade
  (3) sudo apt-get install finger (ouput informaion about a user)

3. Firewall setting
  (1) sudo ufw status numbered (inactivate)
  (2) sudo ufw default deny incoming
  (3) sudo ufw default allow outgoing
  (4) sudo ufw allow ssh (port=22)
  (5) sudo ufw allow 2200/tcp
  (6) sudo ufw allow www (http, port=80)
  (7) sudo ufw allow NTP (port=123)
  (8) sudo ufw enable

4. Change the port for ssh
  (1) sudo nano /etc/ssh/sshd
      port 22 -> 2200
      PasswordAuthentication yes -> no
  (2) sudo service ssh restart
  (3) sudo ufw status numbered
  (4) sudo ufw delete 1 (If you can access the server with the port of 2200, you can delete 22).
  (5) sudo ufw reload

5. Add user, grader
  (1) sudo adduser grader (passwd=grader)
  (2) sudo echo "grader ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/grader (sudo permission for grader)
  (3) ssh-keygen (create public/private rsa key pair)
      /home/ubuntu/.ssh/id_rsa
      id_rsa (private key)
      id_rsa.pub (public key, for server)
  (4) sudo su - grader (login as grader)
  (5) mkdir .ssh
  (6) sudo cp /home/ubuntu/.ssh/id_rsa.pub .ssh/authorized_keys
  (7) sudo chmod 700 .ssh
  (8) sudo chmod 644 .ssh/authorized_keys

6. Time zone setting
  (1) timezonectl (confirm time zone)
  (2) timezonectl list-timezones
  (3) timezonectl set-timezone UTC (if the time zone is not UTC)

7. Install softwares (apache2,libapache2-mod-wsgi,python-setuptools,postgresql)
  (1) sudo apt-get install apache2
  (2) sudo apt-get install libapache2-mod-wsgi (for python2)
  (3) sudo apt-get install python-setuptools
  (4) sudo service apache2 restart
  (5) sudo apt-get install postgresql
  (6) sudo cat /etc/postgresql/9.5/main/pg_hba.conf
      sudo cat /etc/postgresql/9.5/main/postgresql.conf
      (to see if remote connect is not available)
  (7) sudo systemctl restart postgresql

8. Create catalog db
  (1) sudo su - posres
  (2) psql
  (3) CREATE DATABASE catalog;
  (4) CREATE USER catalog;
  (5) ALTER ROLE catalog WITH PASSWORD 'hiking'
  (6) GRANT ALL PRIVILEGES ON DATABASE catalog TO catalog;
  (7) CNTL+D x 2 (logout)

9. Install softwares (git, python-psycopg2, python, python-pip)
  (1) sudo apt-get install git (to clone my remote repository)
  (2) sudo apt-get install python-psycopg2
  (3) sudo apt-get install python (ver. 2.7.12)
  (4) sudo apt-get install python-pip (python package management)
  (5) sudo pip install flask, sqlalchemy, oauth2client, requests

10. Configuration and Script Modification
  (1) sudo a2enmod wsgi (enable the mod_wsgi)
  (2) cd /var/www
  (3) mkdir catalog
  (4) cd catalog (pwd:/var/www/catalog)
  (5) sudo nano catalog.wsgi (create wsgi file)
      #!/usr/bin/python
      import sys
      import logging
      logging.basicConfig(stream=sys.stderr)
      sys.path.insert(0,"/var/www/catalog/")

      from catalog import app as application
      application.secret_key = 'super_secret_key'
  (6) git clone https://github.com/nob496/catalog (clone my remote repository)
  (7) python file modifications
      aplication.py -> __init__.py (rename)

      34: CLIENT_ID = json.loads(open('client_secrets.json', 'r').read())['web']['client_id']
      ->  CLIENT_ID = json.loads(open('/var/www/catalog/catalog/client_secrets.json', 'r').read())['web']['client_id']

      38: engine = create_engine('sqlite:///hikingtrailinfo.db', connect_args={'check_same_thread': False})
      ->  engine = create_engine('postgresql+psycopg2://catalog:hiking@localhost/catalog')
                                 #dialect+driver://username:passwd@host:port/database

      65: app_id = json.loads(open('fb_client_secrets.json', 'r').read())['web']['app_id']
          app_secret = json.loads(open('fb_client_secrets.json', 'r').read())['web']['app_secret']
      ->  app_id = json.loads(open('/var/www/catalog/catalog/fb_client_secrets.json', 'r').read())['web']['app_id']
          app_secret = json.loads(open('/var/www/catalog/catalog/fb_client_secrets.json', 'r').read())['web']['app_secret']

      165:oauth_flow = flow_from_clientsecrets('client_secrets.json', scope='')
      ->  oauth_flow = flow_from_clientsecrets('/var/www/catalog/catalog/client_secrets.json', scope='')

      database_setup.py

      73: engine = create_engine('sqlite:///hikingtrailinfo.db')
      ->  engine = create_engine('postgresql+psycopg2://catalog:hiking@localhost/catalog')

      hikingtrails.py

      06: engine = create_engine('sqlite:///hikingtrailinfo.db')
      ->  engine = create_engine('postgresql+psycopg2://catalog:hiking@localhost/catalog')

   (8) get domain name (hikingdayswithfriends.com, A-IPV4 address/canonical name with www) by AWS route 53 and assign the public IP to the domain
   (9) change google/facebook credential files
       Google developer console (you can also assign domain with xip.io)
       add http://www.hikingdayswithfriends.com to JavaScript/Redirect URL
       add http://www.hikingdayswithfriends.com to client_secrets.json

       Facebook developer
       add http://www.hikingdayswithfriends.com to URL

   (10) sudo nano /etc/apache2/sites-available/catalog.conf (create a new conf file)
        <VirtualHost *:80>
		       ServerName hikingdayswithfriends.com
		       ServerAdmin nob55496@gmail.com
		       WSGIScriptAlias / /var/www/catalog/catalog.wsgi
		       <Directory /var/www/catalog/catalog/>
			        Order allow,deny
			        Allow from all
		       </Directory>
		       Alias /static /var/www/catalog/catalog/static
		       <Directory /var/www/catalog/catalog/static/>
			        Order allow,deny
			        Allow from all
		       </Directory>
		       ErrorLog ${APACHE_LOG_DIR}/error.log
		       LogLevel warn
		       CustomLog ${APACHE_LOG_DIR}/access.log combined
        </VirtualHost>
    (11) sudo a2dissite 000-default.conf
    (12) sudo a2ensite catalog.conf
    (13) sudo python database_setup.py (create catalog.db)
    (14) sudo python hikingtrails.py  (update catalog.db)
    (15) sudo service apache2 reload
    (16) sudo service apache2 restart

:* 11. Additional Changes for 2nd Commit
    (1) sudo /etc/update-motd.d/90-updates-available (check #packages available to be updated)
    (2) cat /etc/apt/sources.list (check the package list for update)
    (3) sudo apt-get update
    (4) sudo apt-get upgrade
    (5) cat /etc/ssh/sshd_config | grep PermitRootLogin
    (6) sudo nano /etc/ssh/sshd_config
        PermitRootLogin prohibit-password -> no (safer option)

        Note:PermitRootLogin (http://manpages.ubuntu.com/manpages/xenial/en/man5/sshd_config.5.html)
         Specifies whether root can log in using ssh(1).  The argument must be “yes”,
         “prohibit-password”, “without-password”, “forced-commands-only”, or “no”.  The
         default is “prohibit-password”.

         If this option is set to “prohibit-password” or “without-password”, password and
         keyboard-interactive authentication are disabled for root.

         If this option is set to “forced-commands-only”, root login with public key
         authentication will be allowed, but only if the command option has been specified
         (which may be useful for taking remote backups even if root login is normally not
         allowed).  All other authentication methods are disabled for root.

         If this option is set to “no”, root is not allowed to log in.

    (7) sudo service ssh restart

References:
 https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
 https://mudspringhiker.github.io/deploying-a-flask-web-app-on-lightsail-aws.html
 https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-using-route-53-to-point-a-domain-to-an-instance
