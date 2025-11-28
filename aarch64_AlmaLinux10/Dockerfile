FROM arm64v8/almalinux:10

RUN dnf install -y \
    'dnf-command(config-manager)' \
    epel-release \
    && dnf config-manager --set-enabled crb \
    && dnf clean all

RUN dnf install -y make rpm-build rpmlint yum-utils && dnf clean all
