FROM ubuntu:14.04.3
MAINTAINER Giovanni Bassi <giggio@giggio.net>

WORKDIR /
RUN sh -c 'echo "deb [arch=amd64] http://apt-mo.trafficmanager.net/repos/dotnet/ trusty main" > /etc/apt/sources.list.d/dotnetdev.list' \
    && apt-key adv --keyserver apt-mo.trafficmanager.net --recv-keys 417A0893 \
    && apt-get update
RUN apt-get install dotnet-nightly -y

ENTRYPOINT ["/bin/bash"]
