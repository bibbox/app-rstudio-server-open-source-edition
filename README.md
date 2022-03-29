# RStudio Server BIBBOX application
BIBBOX App of RStudio server open source addition

This container can be installed as [BIBBOX APP](https://bibbox.readthedocs.io/en/latest/ "BIBBOX") or standalone.
 
After the installation follow these [instructions](INSTALL-APP.md)

## Install within BIBBOX

Within BIBBOX you can use the [BIBBOX](https://bibbox.readthedocs.io/en/latest/ "BIBBOX") to install a lot of software tools. After the installation is finished you can start your application in the dashboard.

### Install Environment Variables
 * USER = username
 * PASSWORD = user password
 
The default values for the standalone installation are:

 * USER = rstudio
 * PASSWORD = rstudio


## Docker Images Used
 * [bibbox/rstudio-server-open-source-edition](https://hub.docker.com/repository/docker/bibbox/rstudio-server-open-source-edition/)
 
## Standalone Installation

To install the app locally execute the commands:
* Clone the git repository: 
  * `git clone https://github.com/bibbox/app-rstudio-server-open-source-edition.git`
* Change the current directory to app-shiny-server: 
  * `cd app-rstudio-server-open-source-edition/` 
* Create the docker network `bibbox-default-network`: 
  * `docker network create bibbox-default-network`
* Run **docker-compose up** in the root folder of the project: 
  * `docker-compose up -d`
* **Alternatively** on a *Linux* system run the bash script `intsall.sh` after cloning and change the working directory to the git repository directory.
 

After the installation (might take a few minutes) open **http://localhost:8787** in your browser to access Shiny.

## Mounted Volumes
* ./data/

