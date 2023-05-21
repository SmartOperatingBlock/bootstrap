# Bootstrap
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

The bootstrap of the project.

The bootstrap repository allows you to deploy the event-broker and all the microservices of the Smart Operating Block at the same time.


## Prerequisites
- Make sure you have a running and active version of *Docker* and *docker-compose*.

## Usage:

1. Clone the repo
2. Create a `.env` file in the root directory with the following variables:
   - `AZURE_CLIENT_ID`: ID of an Azure AD application
   - `AZURE_TENANT_ID`: ID of the application's Azure AD tenant
   - `AZURE_CLIENT_SECRET`: the application's client secrets
   - `AZURE_DT_ENDPOINT`: the Azure Digital Twins instance endpoint
   - `BUILDING_MANAGEMENT_MONGODB_URL`: the mongodb's connection string for the building management microservice
   - `PATIENT_MANAGEMENT_MONGODB_URL`: the mongodb's connection string for the patient management microservice
   - `SIGNALR_CONNECTION_STRING`: connection string of signalR service
   - `STAFF_TRACKING_MONGODB_URL`: the mongodb's connection string for the staff tracking microservice
   - `SURGICAL_PROCESS_MONGODB_URL`: the mongodb's connection string for the surgical process monitoring microservice
   - `SURGERY_REPORT_MONGODB_URL`: the mongodb's connection string for the surgery report microservice
   - `USER_MANAGEMENT_MONGODB_URL`: the mongodb's connection string for the user management microservice
3. Edit the config file for the Automation management microservice in the `config` folder, or leave it as is if you are ok with the default settings. *Note: The file name must be `config.yml`.*
4. Run the following command:
   ```bash
   docker-compose up -d
   ```

