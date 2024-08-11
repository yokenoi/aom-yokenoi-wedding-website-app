# Aom and Yokenoi Wedding Website Application

Website appliation for Aom and Yokenoi wedding.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Deployment](#deployment)

## Introduction

The website application are used for providing information of our wedding and E-card. The webiste provides basic information including the hotel, bride and groom's photos gallery, and wedding location. E-card are used as RSVP for remote guess.

The website is deployed on [Google Cloud Platform](https://cloud.google.com/) via [Cloud Run](https://cloud.google.com/run).

## Installation

The application can be installed depending on the preference of users.

- [Local installation](#local-installation)
- [Container installation](#container-installation)

### Local installation

To install the application, please install [Node.js](https://nodejs.org) on your local machine.

Once [Node.js](https://nodejs.org) is installed, clone this repository on your local machine and run the following command.

```[bash]
npm install
npm run dev
```

Link to application in local will be [`http://localhost:5173/`](http://localhost:5173/).

### Container installation

Please install [Docker](https://www.docker.com) before running the image.

Clone the repository on your local machine and run the following command in the directory.

```[bash]
# Create image
docker build . --tag wedding-website

# Run image
docker run -p 3000:5173 wedding-website
```

Link to application in local will be [`http://localhost:5173/`](http://localhost:5173/).

## Deployment

CI/CD process will be set up to automatically deploy the website to Google Cloud Platform.

Merge `develop` to `master` branch to deploy website to Google Cloud Platform.
