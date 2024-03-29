# restapi-go

## Introduction

This Golang rest api will provide different info based on the route

## Getting Started

To run this project locally and set up a Docker container, follow the steps below:

### Prerequisites

- Install [Docker](https://docs.docker.com/get-docker/)

### Clone the Repository

```bash
git clone git@github.com:chandrasekharkolla/restapi-go.git
cd restapi-go
```

### Initialize Go Modules
Run the following command to initialize Go modules and create the go.mod file:

```bash
go mod init restapi
```
It downloads Dependencies that are required for the restapi
Execute the following command to download and tidy up project dependencies:

```bash
go mod tidy
```
Build the doker image
Build the Docker image with the following command:
```bash
docker build -t <imagename> .
```
Start a Docker container in detached mode, mapping port 8080:
```bash
docker run -d -p 8080:8080 <imagename>
```
Access the Application
Visit http://localhost:8080 in your browser to access the application. Explore various routes as configured in the main.go file.