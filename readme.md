# Laravel Docker

## Installation

Git clone and go project folder
```sh
git clone https://github.com/thetminnhtun-scm/laravel-docker.git laravel-docker
cd laravel-docker
```

Build docker image
```sh
docker-compose build
```

Create and start containers
```sh
docker-compose up -d
```

Install laravel
```sh
cd src
composer create-project laravel/laravel .
```

Open on brower
```sh
http://localhost:8080
```

Done.
