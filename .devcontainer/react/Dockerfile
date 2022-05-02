FROM node:18.1.0-bullseye
WORKDIR /workspace
# apt install
RUN apt update && \
  apt install -y \
  vim \
  bash-completion
# .bashrc
RUN echo '. /etc/bash_completion' >> /etc/bash.bashrc && \
  echo 'source /etc/bash_completion.d/git-prompt' >> /etc/bash.bashrc && \
  echo 'PS1='"'"'${debian_chroot:+($debian_chroot)}\[\\e[1;32m\]\u@\h\[\\e[0m\]:\[\\e[1;33m\]\w\[\\e[1;36m\]$(__git_ps1)\[\\e[0m\]$ '"'" >> /etc/bash.bashrc
