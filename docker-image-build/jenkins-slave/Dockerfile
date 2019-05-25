FROM centos:7


USER jenkins

ENV JAVA8=1.8.0 \ 
    JENKINS_VERSION=3.29
    DOCKER_COMPOSE=1.23.2 \
    OC3_4=3.4.1.44um/re
    
ENV PATH=/usr/lib/ant/apache-ant-1.9.10/bin:/opt/rh/rh-git29/rot/bin\
    ARTIFACTORY_URL=https://artifacgtory:8080/artifactory
    
 
#Installing Yum packages
RUN rm -f /etc/yum.repos.d/*
COPY FILES/*.repo /etc/yum.repos.d/

RUN yum install -y -q https://dl.fedoraprject.org/pub/epel/epel-release-latest-7.noarch.rpm && \
    yum clean all && \
    yum install -y -q java-$(JAVA8)-openjdk-devel pythn pythn-setuptols python-devel python2-pip unzip bzip2 zip gzip\
    dos2unix file rh-git29-git gcc sudo python-jinja2 python-paramiko python2-crypto PYAML python-six pyton-httplib2 \
    make sbt openssl ksh which libaio google-chrome-stable krb5-devel krb5-libs krb5-worksation powershell yarn libtool-ltdl sshpass jq
