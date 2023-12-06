FROM ppc64le/almalinux:8

RUN dnf install -y \
    'dnf-command(config-manager)' \
    epel-release \
    && dnf config-manager --set-enabled powertools \
    && dnf clean all

RUN dnf install -y make rpm-build yum-utils && dnf clean all
