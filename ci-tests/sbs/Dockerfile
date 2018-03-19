FROM scratch
MAINTAINER Jacek Danecki <jacek.m.danecki@gmail.com>
ADD sbs-docker-x86_64.tar.xz /
COPY group /etc
COPY nsswitch.conf /etc
COPY passwd /etc
COPY services /etc
RUN cd / ; while true; do mkdir test1234567890 ; if [ "$?" != "0" ] ; then break ; fi ; cd test1234567890; pwd; done  ; cd / ; rm -rf test1234567890 ; true
RUN cd / ;  rm -rf test1234567890 ; true
RUN cd / ; mv test1234567890 t1
RUN cd / ;  rm -rf t1; true
RUN cd / ; ls -l 
RUN cd / ; ls -l  t1
RUN uname -a
CMD ["/bin/bash"]

