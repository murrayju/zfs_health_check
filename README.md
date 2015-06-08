# zfs_health_check
A cron script to send email notifications when a zpool is in trouble

## Quick start
1. Configure `sendmail` on your system to actually send emails
  * [This guide](https://community.runabove.com/kb/en/instances/how-to-relay-postfix-mails-via-smtp.gmail.com-on-ubuntu-14.04.html) describes how to configure postfix on Ubuntu
2. Edit `zfs_health_check.sh` to configure what email address to send messages to
3. Configure the script to run as a cronjob

  ```
  sudo ln -s /path/to/zfs_health_check.sh /etc/cron.hourly/zfs_health_check
  ```
