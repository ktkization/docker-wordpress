# Docker Wordpress Stack

## Setup

- Install Docker for your platform using instructions from https://docs.docker.com/get-docker/

- Clone the repo
```
$ git clone git@github.com:ktkization/docker-wordpress.git
```

- Create a `.env` file at the root of the project with the following environment variables filled with your preferred values
```
DB_ROOT_PASSWORD=somesecuredbrootpassword
DB_USER=somedbusername
DB_PASSWORD=somesecuredbpassword
DB_NAME=somedbname
```

## Usage

- To run the Wordpress stack execute
```
$ cd docker-wordpress
$ docker-compose up -d
```

- Navigate to http://localhost:8080/ to access `Wordpress` and follow the prompts to setup.
- Navigate to http://localhost:8081/ to access `phpMyAdmin`. Use the credentials in `.env` to access the database.
