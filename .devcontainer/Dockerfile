FROM debian

RUN \
  apt-get update \
  && \
    DEBCONF_NONINTERACTIVE_SEEN=true \
    DEBIAN_FRONTEND=noninteractive \
    apt-get install -y --no-install-recommends \
      busybox-static \
      git \
      less \
      mc \
      procps \
      ssh \
      sudo \
      traceroute \
      wget \
      xz-utils \
  && apt-get clean all
