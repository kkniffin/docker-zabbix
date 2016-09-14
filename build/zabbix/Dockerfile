FROM monitoringartist/zabbix-3.0-xxl
RUN yum install -yq msmtp
RUN echo 'cd /usr/local/share/zabbix/alertscripts && curl -O https://gist.githubusercontent.com/ramunasd/4250117/raw/4744db96cae5af2ddbff953e9920cf79b5b8e636/zext_msmtp.sh && chmod 755 zext_msmtp.sh' >> /etc/rc.local
RUN echo -e 'account zabbix\nhost <mailhost>\ndomain <domain>\nfrom zabbix@<domain>' > /etc/msmtprc
CMD ["/config/bootstrap.sh"]

