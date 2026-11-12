FROM debian

RUN \
  apt-get update \
  && \
    DEBCONF_NONINTERACTIVE_SEEN=true \
    DEBIAN_FRONTEND=noninteractive \
    apt-get install -y --no-install-recommends \
      bind9-dnsutils \
      busybox-static \
      git \
      iproute2 \
      iputils-ping \
      less \
      mc \
      net-tools \
      procps \
      ssh \
      sudo \
      traceroute \
      wget \
      xz-utils \
  && apt-get clean all
