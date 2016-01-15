---
layout: post
title: Disable A Service
about: Disabling a service prevents the cPanel &amp; WHM restart scripts (e.g. restartsrv_mail) from managing the service. It also prevents the cPanel &amp; WHM health monitoring system from managing the service. On CentOS 5, and CentOS 6 systems the services are still managable via the init scripts.
date: 2016-01-03
---

* DNS Daemons: /etc/nameddisable
* FTP Daemons: /etc/ftpddisable or /etc/ftpserverdisable
* Apache: /etc/httpddisable or /etc/apachedisable or /etc/httpdisable
* Dovecot: /etc/imapdisable or /etc/imapddisable or /etc/cpimapdisable or /etc/popdisable or /etc/cppopdisable
* PostgreSQL: /etc/postgresqldisable or /etc/postgresdisable
* rsyslogd: /etc/rsyslogddisable or /etc/rsyslogdisable
* Tailwatch: /etc/tailwatchddisable or /etc/tailwatchdisable

In general you can prevent cPanel &amp; WHM from managing, or acknowledging a service by creating a file in /etc named servicenamedisable or servicenameisevil.