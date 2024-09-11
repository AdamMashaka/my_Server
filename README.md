# Welcome to our Server config script🐕‍🦺!

![image](https://github.com/user-attachments/assets/e2be45b1-f334-4eec-997f-b7ef8232c49b)


## Step 1 
Update, Upgrade, Install web server nginx and python WSGI (Web Server Gateway Interface) Gunicorn
```
sudo apt update && sudo apt upgrade
```

```
sudo apt install nginx
```
```
sudo apt install gunicorn
```

## step 2
Configure nginx and gunicorn (wsgi)
gunicorn.service name your choice

nano /etc/systemd/system/name.service

```
[Unit]
Description=gunicorn daemon
After=network.target

[Service]
User=username
Group=www-data
WorkingDirectory=/path/to/project/
ExecStart=/path/to/virtualenv/ --workers 3 --bind unix:/path/to/sockfile/file.sock mainapp_name.wsgi:application

[Install]
WantedBy=multi-user.target
```


configure nginx

nano /etc/nginx/sites-available/example.com

```
server {
    listen 80;
    server_name 157.173.105.219;  # Replace with your domain or server IP

    location / {
        proxy_pass http://unix:/var/www/client/livescore_yetu/client.sock;  # Point to Gunicorn socket
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
    }

    location /static/ {
        alias /var/www/client/livescore_yetu/static/;  # Path to your Django static files
    }

    location /media/ {
        alias /var/www/client/livescore_yetu/media/;   # Path to your Django media files
    }

    # Logging (Optional)
    access_log /var/log/nginx/adam.access.log;
    error_log /var/log/nginx/adam.error.log;
}
```
