FROM centos:centos7

MAINTAINER nimmis <kjell.havneskold@gmail.com>

ADD jdk-7u71-linux-x64.rpm /

RUN yum localinstall -y /jdk-7u71-linux-x64.rpm && \
rm -f /jdk-7u71-linux-x64.rpm && \
yum clean all

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /root

# Define default command.
CMD ["bash"]

