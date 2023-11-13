# Parcial Docker-Swarm-Rest-Soap
## Ramos Sofia

Aplicación con servicios SOAP y REST, implementados con Node.js y MySQL- Ejecuciòn en contenedores Docker. La aplicación consulta y muestra datos de alumnos a través de servicios SOAP y REST.

## Configuración del Entorno

#### Imagenes
```
* Base de datos - imagen: parcial_swarm_basededatos
* Servicio Rest - imagen: parcial_swarm_rest_service
* Servicio Soap - imagen: parcial_swarm_soap_service 
* Front - imagen: parcial_swarm_front_service
```
### Construcciòn de imàgenes

	1)- docker build -t parcial_swarm_basededatos ./bd
 	2)- docker build -t parcial_swarm_rest_service ./rest_service
  	3)- docker build -t parcial_swarm_soap_service ./soap_service
   	4)- docker build -t parcial_swarm_front_service ./front

### inicializar Docker Swarm

	1)- docker swarm init
	2)- docker stack deploy -c docker-compose.yml parcial
