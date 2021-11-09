FROM centos:latest

RUN yum -y install httpd; yum clean all; systemctl enable httpd.service; \
		yum install httpd; \
        firewall-cmd --add-service=http; \
        firewall-cmd --reload; \
        systemctl restart httpd.service; \
        systemctl start httpd.service; \
        systemctl enable httpd.service; \
        yum install php; \
        systemctl restart httpd.service; \
EXPOSE 80
