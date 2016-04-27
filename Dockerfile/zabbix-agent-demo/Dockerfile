FROM centos:centos7
ADD zabbix-2.4.8rc1.tar.gz /
RUN yum install gcc make -y
WORKDIR /zabbix-2.4.8rc1
RUN ./configure --enable-agent && make install
RUN groupadd zabbix && useradd -g zabbix zabbix

#/usr/local/etc/zabbix_agent.conf
