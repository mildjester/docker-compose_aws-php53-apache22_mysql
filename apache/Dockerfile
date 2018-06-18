FROM amazonlinux:2017.03-with-sources

RUN yum update -y \
 && yum install -y vim httpd php php-devel php-mysql php-pdo php-xml

CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]

