FROM centos:centos7

# Install required packages and remove the apt packages cache when done.
RUN yum install -y https://centos7.iuscommunity.org/ius-release.rpm

RUN yum update -y && \
yum -y install sudo epel-release && \
yum clean all && \
yum groupinstall -y "Development Tools" && \
yum install -y \
git \
python36u \
python36u-libs \
python36u-devel \
python36u-pip \
pcre-devel

RUN pip3.6 install pep8 coverage