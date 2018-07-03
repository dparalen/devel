FROM rohanpm/fedora-vagrant:latest

ARG USER_EUID=1001
ARG USER_EGID=1001

RUN echo "Using USER_EUID ${USER_EUID} USER_EGID ${USER_EGID}"
RUN /sbin/usermod -u ${USER_EUID} vagrant
RUN /sbin/groupmod -g ${USER_EGID} vagrant
RUN /bin/chown -R vagrant:vagrant /home/vagrant
