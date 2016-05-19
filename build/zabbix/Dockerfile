FROM zabbix/zabbix-3.0
RUN yum install -q msmtp
RUN wget https://gist.githubusercontent.com/ramunasd/4250117/raw/4744db96cae5af2ddbff953e9920cf79b5b8e636/zext_msmtp.sh -P /usr/local/share/zabbix/alertscripts
CMD ["/config/bootstrap.sh"]
