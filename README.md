## SWARM CON SERVICIOS SOAP Y REST

## PASO 1 Crear las imagenes

## en apiRest
`docker build . -t examen/restapi`
## en apiSoap
`docker build . -t examen/soapapi`
## en client
`docker build . -t examen/client`
## en mysql
`docker build . -t examen/mysql`

## PASO 2 Desplegar los servicios con swarm

`docker swarm init`

`docker stack deploy -c docker-compose.yml mis-servicios`