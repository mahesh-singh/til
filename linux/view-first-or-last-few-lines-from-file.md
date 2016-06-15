#View first or last few lines from file

`$ head /var/log/syslog`
show first 10 line of file

`$ head -n 15 /var/log/syslog`
-n for number of lines


`$ tail /var/log/syslog`
Last 10 lines of a file by default.

`$ tail -n 10 /var/log/syslog`
-n for number of lines

`$ tail -f /var/log/syslog`
Using tail -f you can see everything that is getting added to that file.
