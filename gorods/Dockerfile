FROM golang:1.7

RUN apt-get update -y

RUN apt-get install -y curl libssl-dev libfuse2

RUN curl -O ftp://ftp.renci.org/pub/irods/releases/4.1.10/ubuntu14/irods-dev-4.1.10-ubuntu14-x86_64.deb

RUN dpkg -i irods-dev-4.1.10-ubuntu14-x86_64.deb

RUN curl -O ftp://ftp.renci.org/pub/irods/releases/4.1.10/ubuntu14/irods-icommands-4.1.10-ubuntu14-x86_64.deb

RUN dpkg -i irods-icommands-4.1.10-ubuntu14-x86_64.deb

RUN go get github.com/jjacquay712/GoRODS

CMD ["/bin/bash"]
