FROM centos:7

MAINTAINER nimmis <kjell.havneskold@gmail.com>

ENV JAVA_VERSION_MAJOR=8 \
    JAVA_VERSION_MINOR=144 \
    JAVA_VERSION_BUILD=01 \
    JAVA_URL_HASH=090f390dda5b47b9b721c7dfaa008135 

RUN yum update -y && \
yum install -y wget && \
wget --no-cookies --no-check-certificate \
  --header "Cookie: gpw_e24=http%3A%2F%2Fwww.oracle.com%2Ftechnetwork%2Fjava%2Fjavase%2Fdownloads%2Fjre8-downloads-2133155.html; oraclelicense=accept-securebackup-cookie" \
  "http://download.oracle.com/otn-pub/java/jdk/${JAVA_VERSION_MAJOR}u${JAVA_VERSION_MINOR}-b${JAVA_VERSION_BUILD}/${JAVA_URL_HASH}/jre-${JAVA_VERSION_MAJOR}u${JAVA_VERSION_MINOR}-linux-x64.rpm" && \
yum localinstall -y jre-${JAVA_VERSION_MAJOR}u${JAVA_VERSION_MINOR}-linux-x64.rpm && \
rm -f jre-${JAVA_VERSION_MAJOR}u${JAVA_VERSION_MINOR}-linux-x64.rpm && \
rm -rf /var/cache/yum

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /root

# Define default command.
CMD ["bash"]

