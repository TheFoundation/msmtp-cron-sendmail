# msmtp-cron-sendmail
  sendmail wrapper for msmtp cron (maybe also with others) replacing from adress header with the one specified in /etc/msmtprc ,  therefore you MUST specify a from bla@blub.tld line in /etc/msmtprc


QUICK INSTALL: mv /usr/sbin/sendmail /usr/sbin/sendmail.real;ln -s /etc/custom/msmtp-cron-sendmail/sendmail /usr/sbin/
(or link your sendmail to also react as /usr/sbin/sendmail.real , then link this script to an earlier PATH stage , e.g. /sbin/ )

have fun