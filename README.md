## Ghost Blog

jinglei.me's src is at usr/share/nginx/ghost on server


To run the Ghost in the src dir as production mode

```
NODE_ENV=production pm2 start index.js --name "Ghost"
```

The named default file in this folder is the Nginx config file. It is at /etc/nginx/sites-enabled/

## slides

The slides is based on HTML using Nginx as the reverse proxy.

To update the Nginx configuration

```
scp default root@slides.jinglei.me:/etc/nginx/sites-enabled/
```

The src dir is at

```
/usr/share/nginx/html/mr-slides/
```

After pull the src code, run

```
service nginx restart
```
