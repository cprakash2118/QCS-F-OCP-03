FROM ubi8/ubi:8.3
MAINTAINER "Chandra Prakash cprakash@qcsdclabs.com"
LABEL description="A custom Apache container based on UBI 8"
RUN yum install -y httpd && \
    yum install -y httpd-manual && \
    yum clean all
RUN echo "Hello from Containerfile" > /var/www/html/index.html
EXPOSE 80
CMD ["httpd", "-D", "FOREGROUND"]

