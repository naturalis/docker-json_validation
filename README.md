docker-json_validation
====================

Docker compose file and docker file for running JSON validation PHP code

Persistent volumes
 - "./www:/var/www/html"  
   Filled with php code
 - "./data:/data"
   persistent data volume

webserver runs on port 80, traefik may add SSL to the mix. 

Contents
-------------
Dockerfile creates the naturalis/json_validation container



Instruction building image
-------------
No special instructions
```
docker build -t naturalis/json_validation:0.0.1 .
```

Instruction running docker-compose.yml
-------------

#### preparation
- Copy env.template to .env and adjust variables. 
- Create empty acme.json file `touch acme.json`

````
docker-compose up -d
````

Usage
-------------

````


````

