from ubuntu:trusty
#maintainer: ali@nikneshan.com
RUN echo "Asia/Tehran" > /etc/timezone && dpkg-reconfigure -f noninteractive tzdata && \
    sed -i s/archive/ir.archive/ /etc/apt/sources.list && apt-get update && apt-get dist-upgrade -y && locale-gen fa_IR 

