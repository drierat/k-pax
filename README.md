# svrKpax

svrKpax son unos servicios creados para la interacci�n de diferentes aplicaci�n es.

Estos servicios interact�an mediante unos plugins de elgg y las aplicaciones que sean necear�as

# Requisitos

Para un correcto funcionamiento se necesita:

mysql 5

jboss 4.2.3

php 5

java 1.6

maven 3.0.3 >

# Instalaci�n

La instalaci�n es muy sencilla, primero nos descargamos el proyecto

    git checkout o nos lo descargamos 
    
Una vez descargando configuramos el pom.xml y configuramos donde deplayamos nuestra app. Cuando todo este configurado ejecutamos el siguiente comando

	mvn install

Lo que realiza es descargar todas las librer�as que necesitamos para que funcione la aplicaci�n, una vez descargadas si queremos que se visualice correctamente en eclipse ejecutamos

	mvn eclipse:eclipse

Y por ultimo para crear un deploy nuevo de la app

	mvn -Denv=local clean package

-Denc=local es el entorno donde se ejecuta, puedes crear todos los que quieras, todo esto se configura en pom.xml

# Instalaci�n MYSQL

En la carpeta src/main/resource/sql esta el script de creaci�n de base de datos

En el momento que ya la tengas creada tienes que configurarar los credencia les, en la misma carpeta hay un archivo que se llama srvKpax-ds.xml, lo configuramos con los datos de nuestro servidor.

Este archivo lo guardamos donde deployamos nuestra aplicacion, por ejemplo:

	/home/server/jboss/server/default/deploy/*

# ICIDENCIAS

Si ten�is alguna incidencia no dud�is enviar un correo a vuestro responsable

# LICENSE

Universitat Oberta de catalunya