* brew install docker --cask
* docker-compose up --build -d --remove-orphans
* docker-compose -f manga-downloader.yml up --build -d --remove-orphans
* Hardlinks - https://trash-guides.info/Hardlinks/Hardlinks-and-Instant-Moves/


# Setup
1. change the default save path in qbit settings to - "/data/download"
2. add the root folder in sonarr to - "/data/media/tv"
3. add the root folder in radarr to - "/data/media/movies"
4. Setup sonarr and radarr and connect to prowlarr and qbit.


# Update images
<!-- Pull images -->
docker-compose pull
<!-- Recreate container -->
docker-compose up --build -d --remove-orphans
<!-- Delete unused images -->
docker system prune

<!-- create network: -->
docker network create mynetwork

#vpn details
https://github.com/navilg/media-stack