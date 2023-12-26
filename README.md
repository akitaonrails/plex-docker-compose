# Docker Compose Scripts for Home Server

This repository contains Docker Compose scripts for setting up a home server. The configuration provided is personal and may need to be adjusted according to your specific requirements.

## Prerequisites

- Docker and Docker Compose installed on your server
- SSH access to your server

## Usage

1. Copy all files to your server:

   ```bash
   scp * user@your-server.local:~/docker/
   ```

2. SSH into your server:

   ```bash
   ssh user@your-server.local
   ```

3. Navigate to the `docker` directory:

   ```bash
   cd docker
   ```

4. Run the Docker Compose file:

   ```bash
   docker compose -f infra-docker-compose.yml up -d
   ```

## Configuration

The `.env.sample` file in this repository contains sample environment variables that are used by the Docker Compose scripts. Before running the scripts, you should rename this file to `.env` and update the variables to match your environment.

To rename the file, use the following command:

```bash
mv .env.sample .env
```

After renaming, open the .env file and replace the placeholder values with your actual data. Save the file and proceed with the steps in the Usage section above.
