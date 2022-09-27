
MAGENTO:

Magento 2 necesita de mariaDb y elasticsearch para su funcionamiento.

Este Docker Compose contiene los tres servicios.


DOC:
https://github.com/bitnami/bitnami-docker-magento

DESPLIEGUE:

Para desplegar magento usar el comando

	> docker-compose up

Esto muestra en el terminal toda la secuencia de arranque

Para una llamada diferida:

	>docker-compose up -d


El proceso tarda unos minutos, especialmente con el despliegue inicial.

Se ha configurado para que los voumenes se creen de forma local dentro de la carpeta

	/magento -> contenido de magento
	/db_data -> contenido de las bases de datos
	/elasticsearch -> contenido de elasticsearch.


USO:

La web se despliega en: 
	http://localhost:8080

El acceso al panel de gestión se realiza desde:
	http://localhost:8080/admin

Los datos de acceso al panel de administración son:

	User: magento  / user
	Pass: magento  / bitnami



