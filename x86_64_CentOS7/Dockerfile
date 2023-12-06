FROM centos:7

RUN yum install -y \
    epel-release \
    https://research.cs.wisc.edu/htcondor/repo/current/htcondor-release-current.el7.noarch.rpm \
    && yum clean all

RUN yum install -y make rpm-build yum-utils && yum clean all

#RUN sed -i s/enabled=0/enabled=1/ /etc/yum.repos.d/htcondor-daily.repo

#RUN echo assumeyes=1 >> /etc/yum.conf
