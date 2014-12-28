FROM centos:centos7

MAINTAINER nimmis <kjell.havneskold@gmail.com>

RUN yum localinstall -y http://downloads.arctics.se/oracle_java/jdk-7u71-linux-x64.rpm && \
yum clean all

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /root

# Define default command.
CMD ["bash"]

