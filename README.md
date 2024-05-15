# Imagen de contenedor SonarQube DevOps Básico

Este repositorio provee una imagen personalizada de SonarQube Community v10.5.1 para el curso de entrenamiento DevOps Básico.
La cual configura por defecto un proxy reverso NGINX para habilitar la capa de seguridad a través de SSL
y el uso de las llaves de seguridad configuradas en el directorio nginx del presente repositorio.

## Version

Versión de SonarQube: **Community 10.5.1**

# Dependencias

Antes de iniciar, necesita asegurar que tiene las siguientes dependencias instaladas:

* [Install Docker](http://docs.docker.com/installation/)
* [Install Docker Compose](http://docs.docker.com/compose/install/)

Ahora puedes verificar si la instalación esta bien con los siguientes comandos:

<pre>
docker version
docker-compose --version
</pre>

# Inicio rápido

Ejecute SonarQube con Docker Compose. Docker Compose utiliza el archivo `docker-compose.yml` que describe el entorno.

```bash
git clone https://github.com/rahozindracompany/sonarqube-devops.git
cd sonarqube
docker-compose up
```

Para detener la ejecución de la imagen ejecute el siguiente comando en el directorio sonarqube-devops:

```bash
docker-compose down
```

## Administración de SonarQube

La consola web de administración de SonarQube puede ser accedida en algunas de las siguientes URLs:
https://localhost:9443/

Las credenciales por defecto para la administración de SonarQube son:

- Username: `admin`
- Password: `admin`


# Diagramas técnicos

## Diagrama de componentes

![Diagrama de componentes](/doc/components-diagram-1.png "Diagrama de componentes")

## Diagrama de despliegue

![Diagrama de despliegue](/doc/physical-diagram.png "Diagrama de despliegue")