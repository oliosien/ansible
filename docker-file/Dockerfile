# https://docs.docker.com/engine/reference/builder/

FROM centos:centos8
ENV container docker
RUN yum -y install python36
#pazKWE7CENh9Y --> Intesys123
#pazxOelvoqxz6 --> ansible
RUN useradd -U -m -p pazxOelvoqxz6 ansible
RUN yum -y install openssh-server
RUN yum -y install openssh-clients
#VOLUME [ “/sys/fs/cgroup” ]
CMD ["/usr/sbin/init"]
EXPOSE 22
