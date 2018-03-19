FROM scratch
MAINTAINER Jacek Danecki <jacek.m.danecki@gmail.com>
ADD sbs-docker-x86_64.tar.xz /
COPY group /etc
COPY nsswitch.conf /etc
COPY passwd /etc
COPY services /etc
RUN cd / ; while true; do mkdir test1234567890 ; cd test1234567890; pwd; done  ; cd / ; rm -r test1234567890 ; rm -rf test1234567890
CMD ["/bin/bash"]

