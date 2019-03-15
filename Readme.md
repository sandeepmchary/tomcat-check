How to install tomcat 7 on ubunutu 14.04
# sudo apt-get update
Install tomcat
# sudo apt-get install tomcat7
change java_opts on /etc/default/tomcat7
restart the tomcat7
sudo service tomcat7 restart
--------------------------------
Additional packages
tomcat7-docs tomcat7-admin tomcat7-examples
# sudo apt-get install tomcat7-docs tomcat7-admin tomcat7-examples
-----------------------------------------
Configure Tomcat Web Management Interface
edit etc/tomcat7/tomcat-users.xml
<tomcat-users>
    <user username="admin" password="password" roles="manager-gui,admin-gui"/>
</tomcat-users>
----------------------------------------------
sudo service tomcat7 restart
---------------------------------
http://server_IP_address:8080

----------------------------------------------------------
Tomcat 7 on CentOS 7

1) sudo yum install tomcat
2) edit sudo vi /usr/share/tomcat/conf/tomcat.conf
3) sudo yum install tomcat-webapps tomcat-admin-webapps 
4) edit sudo vi /usr/share/tomcat/conf/tomcat-users.xml
5) start tomcat
6) restart tomcat
7) Enable tomcat
# Tomcat-check
