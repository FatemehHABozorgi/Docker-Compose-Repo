# Docker Compose Repository

Welcome to the Docker Compose Files Repository. This repository contains a collection of Docker Compose files designed to orchestrate multi-container Docker applications. Each file is configured to be easily customizable and ready for deployment in various environments.

## Table of Contents

- [Overview](#overview)
- [Directory Structure](#directory-structure)
- [Requirements](#requirements)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Usage](#usage)
- [Compose Files](#compose-files)
  - [Example Compose Files](#example-compose-files)
- [Contributing](#contributing)
- [License](#license)

## Overview

This repository serves as a centralized collection of Docker Compose files that define and manage complex containerized applications. Each file is designed to simplify the deployment process and can be easily adapted to meet the needs of different environments.

## Directory Structure

```
Docker-Compose-Repo/
├── compose-files/
│   ├── web-app/
│   │   ├── docker-compose.yml
│   │   └── .env
│   ├── database/
│   │   ├── docker-compose.yml
│   │   └── .env
│   └── ...
├── README.md
└── LICENSE
```

- **compose-files/**: Contains individual Docker Compose files for different applications.
- **README.md**: Documentation for the repository.
- **LICENSE**: Licensing information.
  
## Requirements
Before using the Docker Compose files in this repository, ensure that the following prerequisites are met:

- **Docker**: Version 19.03 or later.
- **Docker Compose**: Version 1.15 or later.
- **Environment Variables**: Ensure the .env files are configured correctly for each compose file.
  
## Getting Started
Installation
Clone the repository to your local machine:
```
git clone https://github.com/FatemehHABozorgi/Docker-Compose-Repo.git
cd Docker-Compose-Repo
```
Install Docker and Docker Compose if they are not already installed. Follow the official installation guides for [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/).


## Usage
To start a multi-container application using a Docker Compose file, navigate to the relevant directory and run:

```
docker-compose -f compose-files/web-app/docker-compose.yml up -d
```
To stop the containers, use:

```
docker-compose -f compose-files/web-app/docker-compose.yml down
```
You can also pass environment-specific variables using the .env file located in the same directory as the docker-compose.yml file.

## Customization
You can customize each Docker Compose file to suit your needs by modifying the following:

- **Service Definitions**: Add, remove, or modify services as required.
- **Environment Variables**: Update the .env file with environment-specific configurations.
- **Volumes and Networks**: Configure volumes and networks to manage persistent storage and service communication.
  
## Compose Files
The repository includes Docker Compose files for various use cases. Below are some examples:

### Example Compose Files
web-app/docker-compose.yml: Defines the setup for a web application with a frontend, backend, and database.

database/docker-compose.yml: Configures a standalone database service with persistent storage.

Each compose file is documented with comments explaining the purpose of each service and configuration option.

## Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.

## Author
Created by Fatemeh Haji Agha Bozorgi.
