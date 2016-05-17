#Supervisord process monitoring

Configuration file location for Supervisord
`/etc/supervisord/supervisord.conf`

```
[include]
files = /etc/supervisor/conf.d/*.conf
```

Sample configuration file (`/etc/supervisord/conf.d`) for process monitoring 

```
[program:nodehook]
command=/usr/bin/node /srv/http.js
directory=/srv
autostart=true
autorestart=true
startretries=3
stderr_logfile=/var/log/webhook/nodehook.err.log
stdout_logfile=/var/log/webhook/nodehook.out.log
user=www-data
environment=SECRET_PASSPHRASE='this is secret',SECRET_TWO='another secret'
```


##Controlling the process 