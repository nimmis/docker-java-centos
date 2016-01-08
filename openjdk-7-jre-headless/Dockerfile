FROM centos:7

MAINTAINER nimmis <kjell.havneskold@gmail.com>

RUN yum update -y && \
yum install -y wget && \
yum install -y java-1.7.0-openjdk-headless && \
yum clean all

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /root

# Define default command.
CMD ["bash"]

