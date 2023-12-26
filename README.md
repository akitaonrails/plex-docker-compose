## Docker Compose Scripts for my Home Server

This is my personal config. You will need to tweak it to your needs.

Example of usage:

```
scp * akitaonrails@plex.local:~/docker/
ssh akitaonrails@plex.local
cd docker
docker compose -f infra-docker-compose.yml up -d
```
