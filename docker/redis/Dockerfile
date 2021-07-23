FROM redis:latest
LABEL maintainer="realsnake1975@gmail.com"
VOLUME /tmp

# 보안검수 조치
# RUN rm /usr/bin/curl
RUN groupadd momorydb && useradd uredis -g momorydb
USER uredis

ENTRYPOINT ["docker-entrypoint.sh"]
CMD ["redis-server"]
