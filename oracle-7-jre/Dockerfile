FROM centos:7

MAINTAINER nimmis <kjell.havneskold@gmail.com>


RUN yum update -y && \
yum install -y wget && \
wget https://mirror.its.sfu.ca/mirror/CentOS-Third-Party/NSG/common/x86_64/jre-7u80-linux-x64.rpm && \
yum localinstall -y /jre-7u80-linux-x64.rpm && \
rm -f /jre-7u80-linux-x64.rpm && \
rm -rf /var/cache/yum

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /root

# Define default command.
CMD ["bash"]

