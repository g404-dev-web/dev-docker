## Simplon Roanne Dev Environment with Docker

Dev Environment targeted at french coding school junior devs.

## Stack

PHP7/NodeJS/Nginx/MariaDB/PostgreSQL/MongoDB 

## Requirements

### Docker

[Get Docker CE for Ubuntu | Docker Documentation](https://docs.docker.com/install/linux/docker-ce/ubuntu/)

[Post-installation steps for Linux | Docker Documentation](https://docs.docker.com/install/linux/linux-postinstall/)

Both link setup procedures must be followed. 
And finally the cli docker-compose : 

[Install Docker Compose | Docker Documentation](https://docs.docker.com/compose/install/#install-compose)


### Kitematic

GUI for docker

[Releases · docker/kitematic · GitHub](https://github.com/docker/kitematic/releases)

### Files permissions

```bash
sudo usermod -aG $(whoami) root
```

Run this into ```simplon-dev``` directory : 

```bash
sudo chown -R $(whoami):root public
```

## Setup

```bash
git clone https://github.com/simplon-roanne/dev-docker
```

## HTTP Access to PHP7/Nginx webserver
http://127.0.0.1:22222

## Creating the containers for later user with Kitematic
```bash
docker-compose up --no-start
```

## Creating the containers and running them immediatly
```bash
docker-compose up 
```

