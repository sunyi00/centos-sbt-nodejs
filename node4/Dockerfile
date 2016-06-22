FROM registry.yxapp.xyz/centos:1.0.1

RUN curl https://bintray.com/sbt/rpm/rpm > /etc/yum.repos.d/bintray-sbt-rpm.repo \
    && yum install -y sbt \
    && yum -y clean all

RUN curl -LO https://nodejs.org/dist/v4.4.5/node-v4.4.5-linux-x64.tar.gz \
    && tar --strip-components 1 -xzvf node-v* -C /usr/local \
    && rm -f node-v4.4.5-linux-x64.tar.gz
