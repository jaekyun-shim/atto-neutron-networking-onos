FROM registry.access.redhat.com/rhosp13/openstack-neutron-server
MAINTAINER Atto research team <jaekyun.shim@atto-research.com>

###Required Labels
LABEL name="atto-neutron" \
      maintainer="jaekyun.shim@atto-research.com" \ 
      vendor="atto-research" \
      version="2.0" \
      release="2" \
      summary="Atto-research plugin installed neutron api" \
      description="Atto-research plugin installed version of neutron_api server" 
      

### add licenses to this directory
USER root
RUN mkdir -p /licenses
COPY licensing.txt /licenses

### Add necessary Red Hat repos here
#RUN REPOLIST=rhel-7-server-rpms,rhel-7-server-optional-rpms \

### Add your package needs here
#    INSTALL_PKGS="PACKAGES HERE" && \
#    yum -y update-minimal --disablerepo "*" --enablerepo rhel-7-server-rpms --setopt=tsflags=nodocs \
#     --security --sec-severity=Important --sec-severity=Critical && \
#   yum -y install --disablerepo "*" --enablerepo ${REPOLIST} --setopt=tsflags=nodocs ${INSTALL_PKGS} && \

### Install your application here -- add all other necessary items to build your image
#RUN "ANY OTHER INSTRUCTIONS HERE"

USER neutron
