Key provided above for the SECRET_ENCRYPTION_KEY environment variable is randomly generated using your browser cryotography API. It will be different every time You can generate one yourself using openssl rand -hex 32


Updating

To update, navigate to the directory with the docker-compose.yaml located.

    Stop Homarr using docker compose down
    Pull the newest image of Homarr using docker compose pull
    Start Homarr again using docker compose up -d (-d for detached mode - start in background)
    Delete the old image using docker image prune (Warning: this also removes you other unused images - not just Homarr)

Uninstalling

To uninstall, navigate to the directory with the docker-compose.yaml located.

    Stop Homarr using docker compose down
    Delete the created directories & files on your root file system (check docker-compose.yaml file for your specific locations)
    Delete compose file using rm docker-compose.yaml
    Prune unused Docker images using docker image prune (Warning: this also removes you other unused images - not just Homarr)
    (Optional): Prune any network or volumes if you use any.
    (Optional): Remove Homarr from your reverse proxy, VPNs or tunnels if you use any.

