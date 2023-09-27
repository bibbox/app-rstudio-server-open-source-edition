# rstudio-server-open-source-edition BIBBOX application

This container can be installed as [BIBBOX APP](https://bibbox.readthedocs.io/en/latest/ "BIBBOX App Store") or standalone. 

- after the docker installation follow these [instructions](INSTALL-APP.md)

## Standalone Installation 

Clone the github repository. If necessary change the ports in the environment file `.env` and the volume mounts in `docker-compose.yml`.

```
git clone https://github.com/bibbox/app-rstudio-server-open-source-edition
cd app-rstudio-server-open-source-edition
docker-compose up -d
```

The main app can be opened and set up at
```
http://localhost:8787
```

## Install within BIBBOX

Visit the BIBBOX page and find the App by its name in the Store. Click on the symbol and select Install. Then fill the parameters below and name your app click install again.

## Docker Images used
  - [bibbox/rstudio-server-open-source-edition](https://hub.docker.com/r/bibbox/rstudio-server-open-source-edition) 


 
## Install Environment Variables
  - USER = Username for the first rstudio user
  - PASSWORD = Password for the first rstudio user

  
The default values for the standalone installation are:
  - USER = rstudio
  - PASSWORD = rstudio

  
## Mounted Volumes
### bibbox/rstudio-server-open-source-edition Conatiner
  - *./data:/home*
