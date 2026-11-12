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
      locales \
      mc \
      net-tools \
      procps \
      ssh \
      sudo \
      traceroute \
      wget \
      xz-utils \
  && apt-get clean all

# Make sure 'en_US.UTF-8' locale is available. Expects 'locales' package to be already installed.
RUN \
  sed -E 's/^# (en_US.UTF-8)/\1/i' --in-place /etc/locale.gen \
  && locale-gen
