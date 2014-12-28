FROM centos:centos7

MAINTAINER nimmis <kjell.havneskold@gmail.com>

ADD jre-7u71-linux-x64.rpm /

RUN yum localinstall -y /jre-7u71-linux-x64.rpm && \
rm -f /jre-7u71-linux-x64.rpm && \
yum clean all

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /root

# Define default command.
CMD ["bash"]

