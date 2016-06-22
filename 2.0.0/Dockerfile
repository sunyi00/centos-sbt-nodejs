FROM registry.lain.bdp.cc/centos:1.0.1

RUN curl https://bintray.com/sbt/rpm/rpm > /etc/yum.repos.d/bintray-sbt-rpm.repo \
    && yum install -y sbt \
    && yum -y clean all

RUN https_proxy=antigfw.bdp.cc:3128 curl -LO https://nodejs.org/dist/v5.0.0/node-v5.0.0-linux-x64.tar.gz \
    && tar --strip-components 1 -xzvf node-v* -C /usr/local \
    && rm -f node-v5.0.0-linux-x64.tar.gz
