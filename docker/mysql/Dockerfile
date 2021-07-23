FROM mysql:5.7
LABEL maintainer="realsnake1975@gmail.com"
# ADD ./init.sql /docker-entrypoint-initdb.d
EXPOSE 3306

ENV MYSQL_ROOT_PASSWORD=!@#Root123
# ENV MYSQL_DATABASE=account
# ENV MYSQL_USER=account
# ENV MYSQL_PASSWORD=!@#Account123

# 보안검수 조치
# RUN rm /usr/bin/curl
RUN groupadd rdbms && useradd umysql -g rdbms
USER umysql

ENTRYPOINT ["docker-entrypoint.sh"]
CMD ["mysqld"]
