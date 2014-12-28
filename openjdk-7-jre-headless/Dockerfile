FROM centos:centos7

MAINTAINER nimmis <kjell.havneskold@gmail.com>

RUN yum install -y java-1.7.0-openjdk-headless && \
yum clean all

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /root

# Define default command.
CMD ["bash"]

