# Label-Studio Deployment with Docker Compose and Traefik

This repository demonstrates a robust approach for deploying Label-Studio using Docker Compose and Traefik 3. For comprehensive details about Label-Studio, please refer to the official repository: https://github.com/HumanSignal/label-studio

## Installation Guide

1. **Preparation:**
	- Transfer all repository files to your server.
	- Ensure that Docker Compose and Traefik are installed and configured according to the instructions provided at https://github.com/wollomatic/simple-traefik.

2. **Configuration:**
	- Update the URLs in `docker-compose.yml` to reflect your specific environment and domain settings.
	- Enter your authentication credentials in `.env`.
    - The folder with the label-studio-data should have permission 700 (drwx------) and should be assigned to the user 1001 (This is unfortunately a peculiarity of Label-Studio). Make sure you have not defined user 1001 in Linux!

## Disclaimer

Please be aware that you use this project at your own risk. The author assumes no responsibility or liability for any issues, damages, or losses resulting from the use of this repository. Ensure you understand the configuration and deployment steps before proceeding.

## Acknowledgments

This project builds upon the excellent work at https://github.com/wollomatic/simple-traefik, which provided the foundation for the Traefik integration.