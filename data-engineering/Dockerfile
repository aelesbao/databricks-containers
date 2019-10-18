FROM openjdk:8u212-jdk-alpine3.9

RUN apk add --no-cache \
    bash \
    coreutils \
    fuse \
    monit \
    openssh-server \
    procps \
    sudo

# Warning: the created user has root permissions inside the container
# Warning: you still need to start the ssh process with `sudo service ssh start`
RUN adduser -s /bin/bash -G wheel -D alpine
