FROM amazonlinux:2

RUN yum install -y \
    https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm \
    https://research.cs.wisc.edu/htcondor/repo/current/htcondor-release-current.amzn2.noarch.rpm \
    && yum clean all

RUN yum install -y make rpm-build yum-utils && yum clean all

#RUN sed -i s/enabled=0/enabled=1/ /etc/yum.repos.d/htcondor-daily.repo

#RUN echo assumeyes=1 >> /etc/yum.conf
