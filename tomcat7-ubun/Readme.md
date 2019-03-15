# install tomcat
sudo apt-get update
sudo apt-get install tomcat 7 -y
# config the file /etc/default/tomcat7
JAVA_OPTS="-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -Xmx512m -XX:MaxPermSize=256m -XX:+UseConcMarkSweepGC"
# restart tomcat
sudo service tomcat7 restart
# Install additional packages
 sudo apt-get install tomcat7-docs tomcat7-admin tomcat7-examples
# Configure Tomcat Web Management Interface
/etc/tomcat7/tomcat-users.xml
'''
<tomcat-users>
    <user username="admin" password="password" roles="manager-gui,admin-gui"/>
</tomcat-users>
'''
