#FROM debian:latest
FROM remont
MAINTAINER pers1307 <skulines@mail.ru>

# Не похоже на правильное решение, но пока так
#RUN ["chmod", "+x", "/home/user/start.sh"]

# apache2 up
CMD /usr/sbin/apache2ctl -D FOREGROUND


EXPOSE 3306




#RUN apt-get update && apt-get install -y openssh-server
#RUN mkdir /var/run/sshd

#RUN echo 'root:screencast' | chpasswd
#RUN sed -i 's/PermitRootLogin prohibit-password/PermitRootLogin yes/' /etc/ssh/sshd_config

# SSH login fix. Otherwise user is kicked off after login
#RUN sed 's@session\s*required\s*pam_loginuid.so@session optional pam_loginuid.so@g' -i /etc/pam.d/sshd

#ENV NOTVISIBLE "in users profile"
#RUN echo "export VISIBLE=now" >> /etc/profile

#RUN useradd -m -p '$1$WxsdvPWd$euoLxPQb45TQ7rrDlNWUZ/' user #user

#EXPOSE 22
#CMD ["/usr/sbin/sshd", "-D"]


#CMD ["mysqld_safe"]

# ssh server up
#RUN apt-get update && apt-get -y upgrade && DEBIAN_FRONTEND=noninteractive apt-get -y install \
#    openssh-server
#RUN useradd -m -p '$1$WxsdvPWd$euoLxPQb45TQ7rrDlNWUZ/' user #user
#CMD /usr/sbin/ssh -D FOREGROUND

# MySql up
#RUN chown -R mysql:mysql /var/lib/mysql
#RUN mysql_install_db --user=mysql -ldata=/var/lib/mysql/
#CMD /usr/sbin/mysqld -D FOREGROUND



#ENTRYPOINT /home/user/start.sh
#CMD /home/user/start.sh

#RUN apt-get update && apt-get -y upgrade && DEBIAN_FRONTEND=noninteractive apt-get -y install \
#    openssh-server git mc

##    apache2 php7.0 php7.0-mysql libapache2-mod-php7.0 curl lynx-cur

#RUN useradd -m -p '$1$WxsdvPWd$euoLxPQb45TQ7rrDlNWUZ/' user #user
#RUN systemctl enable ssh.service

#EXPOSE 22


#FROM debian:latest
#MAINTAINER pers307 <skulines@mail.ru>
#
#RUN apt-get update && apt-get -y upgrade && DEBIAN_FRONTEND=noninteractive apt-get -y install \
#    openssh-server git mc
#
##    apache2 php7.0 php7.0-mysql libapache2-mod-php7.0 curl lynx-cur
#
#RUN useradd -m -p '$1$WxsdvPWd$euoLxPQb45TQ7rrDlNWUZ/' user #user
#RUN systemctl enable ssh.service
#
#EXPOSE 22


#apachectl start
#git
#publisher path
#add user


# Install apache, PHP, and supplimentary programs. openssh-server, curl, and lynx-cur are for debugging the container.
#RUN apt-get update && apt-get -y upgrade && DEBIAN_FRONTEND=noninteractive apt-get -y install \
#    apache2 php7.0 php7.0-mysql libapache2-mod-php7.0 curl lynx-cur
#
#RUN apt-get update && apt-get -y install \
#mysql-server mysql-client
#
#RUN apt-get update && apt-get -y install \
#php7.0-gd php-imagick php7.0-curl php-xml
#
# Create user and ssh server for connect in pfone mode
#
# Enable apache mods.
#RUN a2enmod php7.0
#RUN a2enmod rewrite

# Update the PHP.ini file, enable <? ?> tags and quieten logging.
#RUN sed -i "s/short_open_tag = Off/short_open_tag = On/" /etc/php/7.0/apache2/php.ini
#RUN sed -i "s/error_reporting = .*$/error_reporting = E_ALL ^ E_NOTICE ^ E_WARNING E_ERROR | E_WARNING | E_PARSE/" /etc/php/7.0/apache2/php.ini

# Manually set up the apache environment variables
#ENV APACHE_RUN_USER www-data
#ENV APACHE_RUN_GROUP www-data
#ENV APACHE_LOG_DIR /var/log/apache2
#ENV APACHE_LOCK_DIR /var/lock/apache2
#ENV APACHE_PID_FILE /var/run/apache2.pid

# Expose apache.
#EXPOSE 80

# Copy this repo into place.
#ADD www /var/www/site

# Update the default apache site with the config we created.
#ADD apache-config.conf /etc/apache2/sites-enabled/000-default.conf

# By default start up apache in the foreground, override with /bin/bash for interative.
#CMD /usr/sbin/apache2ctl -D FOREGROUND
