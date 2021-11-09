FROM centos:7

RUN yum -y install httpd; yum clean all; systemctl enable httpd.service; \
		yum install httpd; \
        firewall-cmd --add-service=http; \
        firewall-cmd --reload; \
        systemctl restart httpd.service; \
        systemctl start httpd.service; \
        systemctl enable httpd.service; \
EXPOSE 80
