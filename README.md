# Setup Docker for Odoo 16 with pgAdmin Access


### Install docker:
```
$ sudo apt install docker.io
$ sudo systemctl start docker
$ sudo systemctl enable docker
```

### Install docker compose:
```
$ sudo apt-get install curl
$ sudo curl -L "https://github.com/docker/compose/releases/download/2.16.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
$ sudo systemctl enable docker
```

### Resolve permission issue:
```
$ sudo chmod -R 777 addons
$ sudo chmod -R 777 etc
$ mkdir -p postgresql
$ sudo chmod -R 777 postgresql
```

### Start the container from the root of this project:
```
$ docker-compose up  -d
```

Then locate `localhost:16000` to access Odoo 16.0.

<img width="500px" src="https://github.com/Sayed09/odoo-16-docker/blob/main/screenshots/odoo-apps.png" alt="Odoo is working.">

