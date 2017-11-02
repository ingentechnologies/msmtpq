#Ingen MSMTPQ

A simple set of scripts forked from the example scripts of the msmtp mail client.

##Install
1. Create a /usr/local/msmtpq folder and copy the script here
2. Create a world writable directory /usr/local/msmtpq/queue
3. Copy the .service, .timer, .path file into /etc/systemd/system/ folder.
4. Install either or the .timer and .path unit with "systemctl enable msmtp-queue.timer" command.  
5. Install the msmtp package and follow setup instructions: https://blog.joeb454.com/2016/08/configuring-msmtp-on-ubuntu-16-04/ 
6. Create a symlink to /usr/sbin/sendmail to the msmtpq script at /usr/local/msmtpq/msmtpq
7. PHP7 nor Apahce PHP mod should require any special configuration to use since sendmail is replaced.

