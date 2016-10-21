FROM centos:7

ARG MY_DATOMIC_USER
ARG MY_DATOMIC_DOWNLOAD_KEY
ARG DATOMIC_VERSION
ENV DATOMIC_HOME="/opt/datomic-pro-${DATOMIC_VERSION}"
ENV DATOMIC_DATA=$DATOMIC_HOME/data
ENV PATH="${PATH}:${DATOMIC_HOME}/bin"

RUN yum -y update && \
  yum -y install wget && \
	yum -y install tar && \
	yum -y install unzip && \
  yum -y install java-1.8.0-openjdk-headless

RUN wget --http-user=$MY_DATOMIC_USER --http-password=$MY_DATOMIC_DOWNLOAD_KEY https://my.datomic.com/repo/com/datomic/datomic-pro/$DATOMIC_VERSION/datomic-pro-$DATOMIC_VERSION.zip -O /tmp/datomic.zip \
  && unzip /tmp/datomic.zip -d /opt \
  && rm -f /tmp/datomic.zip

ADD config $DATOMIC_HOME/config

WORKDIR $DATOMIC_HOME
VOLUME $DATOMIC_DATA
