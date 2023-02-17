# Bootstrap
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

The bootstrap of the project.

The bootstrap repository allows you to deploy the event-broker and all the microservices of the Smart Operating Block at the same time.


## Prerequisites
- Make sure you have a running and active version of *Docker* and *docker-compose*.

## Usage:

1. Clone the repo
2. Create a `.env` file in the root directory with the following variables:
   - `SIGNALR_CONNECTION_STRING`
   - `USER_MANAGEMENT_MONGODB_URL`
3. Run `docker-compose up -d`

