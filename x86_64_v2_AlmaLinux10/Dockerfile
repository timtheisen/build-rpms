FROM --platform=linux/amd64/v2 almalinux/10-base:10

RUN dnf install -y \
    'dnf-command(config-manager)' \
    epel-release \
    && dnf config-manager --set-enabled crb \
    && dnf clean all

RUN dnf install -y make rpm-build yum-utils && dnf clean all
