FROM alpine
LABEL maintainer=univi@vip.qq.com

# Change repo to aliyun
RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories \
    && apk update \
    && apk add --no-cache bash \
    && rm -rf /var/cache/apk/*

ENTRYPOINT [ "/bin/sh", "-c", "while true; do sleep 60;done" ]
