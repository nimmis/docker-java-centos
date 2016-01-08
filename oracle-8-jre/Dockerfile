FROM centos:7

MAINTAINER nimmis <kjell.havneskold@gmail.com>

RUN yum update -y && \
yum install -y wget && \ 
wget -O /jre-8u66-linux-x64.rpm http://javadl.sun.com/webapps/download/AutoDL?BundleId=111740 && \
yum localinstall -y /jre-8u66-linux-x64.rpm && \
rm -f /jre-8u66-linux-x64.rpm && \
yum clean all

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /root

# Define default command.
CMD ["bash"]

