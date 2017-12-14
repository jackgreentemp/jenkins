FROM jenkins

USER root
#install nodejs
RUN apt-get update \
 && apt-get install -y \
 	curl \
 && curl -sL https://deb.nodesource.com/setup_8.x | bash - \
 && curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg |  apt-key add - \
 && echo "deb http://dl.yarnpkg.com/debian/ stable main" |  tee /etc/apt/sources.list.d/yarn.list \
 && apt-get update  \
 && apt-get install -y nodejs yarn sudo \
 && rm -rf /var/lib/apt/lists/*

RUN curl -sSL https://get.docker.com/ | sh && \
    usermod -aG docker jenkins

# install necessary packages
# RUN apt-get update \
#       && apt-get install -y sudo \
#       && rm -rf /var/lib/apt/lists/*

# 我们需要赋予jenkins用户sudo权限以便能在容器内运行Docker命令
# RUN echo "jenkins ALL=NOPASSWD: ALL" >> /etc/sudoers

# Install initial plugins
# USER jenkins
# COPY plugins.txt /usr/share/jenkins/plugins.txt
# RUN /usr/local/bin/plugins.sh /usr/share/jenkins/plugins.txt
