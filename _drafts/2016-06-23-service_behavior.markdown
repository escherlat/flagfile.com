---
layout: post
title: Service Behavior
about: Files that determine how a particular service behaves when it is running.
date: 2016-06-23
---

* /var/cpanel/noanonftp: when present Anonymous FTP is not available. It also hides the Anonymous FTP functions in the cPanel interface
* /var/cpanel/imap_tcp_check_disabled: when present, prevents chkservd from perform TCP checks of Dovecot
* /var/cpanel/useclusteringdns: when present instructs system that cPanel DNS Clustering is active.
* 