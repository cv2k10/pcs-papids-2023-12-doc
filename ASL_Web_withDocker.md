## Project Title
# LRT3-PAPIDS Web (Compiled build with docker)

## Table of Content:

- [About The App](#about-the-app)
- [Setup Files](#screenshots)
- [Installation folders](#technologies)
- [Installation Steps](#react-app-setup)

## About The App
LRT3-PAPIDS Front End System docker installation files for each LRT station


## Setup Files
The docker installation file is located in the C:\pcs-lrt3-release location on the testing workstation in the PCS office.
![web-docker-setup-files](web-docker-setup-files.png)


## Installation folders
Each of the docker installation folder consists of 2 docker images, one is ping-server image and the other is web-server image.

The ping-server image was built by the source code of ASLPingServer https://github.com/PCS-GIS-PAPIDS-Control-Software/ASLPingServer

The web-server image was built by the source code of ASL_Web https://github.com/PCS-GIS-PAPIDS-Control-Software/ASL_Web

All the station uses the same ping-server image, whereas there is different web-server images for each of the station.

These docker installation folder is the front-end web setup for the LRT station, which should be installed on the workstation of LRT station.

## Installation Steps

1. Copy the correct folder for selected station to a folder named papids-web on root drive c:
2. Open the command terminal
2. Go into the folder, by typing ```cd c:/papids-web``` on the command terminal
3. Start docker installation by typing ```docker compose up -d``` on the command terminal
4. Wait to complete the whole installation process


