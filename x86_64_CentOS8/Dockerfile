FROM centos:8

RUN dnf install -y \
    'dnf-command(config-manager)' \
    epel-release \
    https://research.cs.wisc.edu/htcondor/repo/current/htcondor-release-current.el8.noarch.rpm \
    && dnf config-manager --set-enabled powertools \
    && dnf clean all

RUN yum install -y make rpm-build yum-utils && yum clean all

#RUN sed -i s/enabled=0/enabled=1/ /etc/yum.repos.d/htcondor-daily.repo

#RUN echo assumeyes=1 >> /etc/yum.conf
