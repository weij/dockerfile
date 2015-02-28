FROM java:8

MAINTAINER Weijun Yin <weijun.yin@gmail.com>

ENV KIBANA_VERSION 4.0.0-linux-x64

RUN curl https://download.elasticsearch.org/kibana/kibana/kibana-${KIBANA_VERSION}.tar.gz | tar zx -C /opt

ADD ./run.sh /run.sh
RUN chmod +x /run.sh

EXPOSE 5601

ENTRYPOINT /run.sh
