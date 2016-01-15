---
layout: post
title: Mail Configuration
about: Flag files used for configuring behavior of the mail system exim or dovecot.
date: 2016-01-03
---

/etc/eximmailtrap

:    Adds X-Source email header to outgoing mail

/etc/webspam

:          Prevent the &apos;nobody&apos; user from sending mail
          
/etc/popbeforesptmp

:         Allow use of POP-before-SMTP for authentication

/etc/eximpopbeforesmtpwarning

:         Adds the system user name (or list of user names) that sent an email to the X-PopBeforeSMTPSenders header

/var/cpanel/allow_domainowner_mail_pass

:         When present allows the cPanel user to masquerade as an email account via IMAP and SMTP

/var/cpanel/email_send_limits/count_mailman

:          When present include Mailman mailing list messages in Mail sending limits calculations

/var/cpanel/smtpgidonlytweak

:          When present restrict sending of email to exim only.

/etc/global_spamassassin_enable

:          When present SpamAssassin is enabled for all accounts

/var/cpanel/config/email/trust_x_php_script

:          Use the X-PHP-Script to determine who sent a message

/var/cpanel/config/email/query_apache_for_nobody_senders

:          Query the webserver to determine who sent a message. Potentially an expensive operation.

/var/cpanel/custom_mailips

:          Exi will use contents of <em>/etc/mailips</em> to determine which IPv4 address to use for outbound connections for an account

/var/cpanel/exim_ipv4_sort_bias

:          Instructs Exim to prefer sending to an IPv4 address versus an IPv6 address