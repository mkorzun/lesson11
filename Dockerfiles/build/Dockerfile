FROM maven:3.8.4-jdk-8
RUN apt update -y && apt install -y git docker.io openssh-client && apt remove --purge --auto-remove -y
COPY stage /root/.ssh/id_rsa
COPY config.json /root/.docker/config.json
RUN chmod 600 /root/.ssh/id_rsa
RUN chmod 600 /root/.docker/config.json