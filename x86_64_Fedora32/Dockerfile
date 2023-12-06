FROM fedora:32

RUN yum install -y https://research.cs.wisc.edu/htcondor/repo/current/htcondor-release-current.fc32.noarch.rpm && yum clean all

RUN yum install -y make rpm-build yum-utils && yum clean -y all

#RUN sed -i s/enabled=0/enabled=1/ /etc/yum.repos.d/htcondor-daily.repo

#RUN echo assumeyes=1 >> /etc/yum.conf
