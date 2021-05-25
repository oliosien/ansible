# https://docs.docker.com/engine/reference/builder/

FROM centos:centos8
ENV container docker
RUN yum -y install python36
#pazKWE7CENh9Y --> Intesys123
#pazxOelvoqxz6 --> ansible
RUN useradd -U -m -p pazxOelvoqxz6 ansible
RUN yum -y install openssh-server
RUN yum -y install openssh-clients
RUN yum -y install httpd
RUN yum -y install telnet
RUN yum -y install sudo
RUN yum -y install python3-lxml
RUN usermod -aG wheel ansible
CMD ["/usr/sbin/init"]
#CMD service httpd start
EXPOSE 22 80 8080 9090
