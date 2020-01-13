FROM dhawton/base

RUN apk-install nodejs && \
  find /var/lib/apk/ -mindepth 1 -delete && \
  find /tmp/ /var/log/ -mindepth 1 -delete && \
  rm -rf /root/.cache && \
  docker-run-bootstrap && \
  docker-image-cleanup