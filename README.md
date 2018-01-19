
# rpi-rental-solution
A dockerized solution for downloading through OpenVPN through Transmission with Sonarr and Radarr.

# Volume mounts

#### Should be mounted to the host file system prior to starting containers

/mnt/downloads - Transmission's dump location

/mnt/tv - Sonarr scans and puts finished episodes here

/mnt/movies - Radarr scans and puts finished movies here

#### Should be created using the docker `docker volume create VOL` command, but can be mapped mounted anywhere else as long as the docker-compose.yml is changed accordingly.
sonarr_config

radarr_config

# Reminder
Check all environment variables to ensure they match in your use-case.