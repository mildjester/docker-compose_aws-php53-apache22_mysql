FROM mysql:5.6

RUN sed -ie "s/mysql:x:999:999/mysql:x:1000:1000/g" /etc/passwd \
 && sed -ie "s/mysql:x:999/mysql:x:1000/g" /etc/group \
 && chown -R mysql:mysql /var/lib/mysql \
 && chown -R mysql:mysql /var/lib/mysql-files \
 && chown -R mysql:mysql /var/lib/mysql-keyring

WORKDIR /var/lib/mysql
