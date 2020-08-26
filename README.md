# msmtp-cron-sendmail
  sendmail wrapper for msmtp cron (maybe also with others) replacing from adress header with the one specified in /etc/msmtprc ,  therefore you MUST specify a 

> msmtp ( and maybe others) wrapper for cron , 
> changing the from Field to a valid mail address
> Inspired by https://marlam.de/msmtp/old-mailinglist/msg00942.html

`from bla@blub.tld `

line in /etc/msmtprc


QUICK INSTALL: mv /usr/sbin/sendmail /usr/sbin/sendmail.real;ln -s /etc/custom/msmtp-cron-sendmail/sendmail /usr/sbin/


(or link your sendmail to also react as /usr/sbin/sendmail.real , then link this script to an earlier PATH stage , e.g. /usr/local/sbin/ )


##example working on debian 9:(and noninvasive) - reason: /usr/local/sbin/ is first in path, regular sendmail in /usr/sbin

ln -s /etc/custom/msmtp-cron-sendmail/sendmail /usr/local/sbin/;ln -s /usr/sbin/sendmail /usr/sbin/sendmail.real

have fun

