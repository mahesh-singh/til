#uwsgi nginx configuration

```
server {
    listen 80;
    server_name client.maheshsingh.org;

        location / {
        include uwsgi_params;
        uwsgi_pass unix:/tmp/mitushi.sock;
    }
}
```
