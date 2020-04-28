# CASO ESTUDIO ALQUILER DE VIDEOS

Para el problema considere al menos las siguientes transacciones (puede incluir otras):
* Administrar Clientes
* Administrar Videos
* Registrar alquiler de video
* Registrar devolución de video
* Reporte de alquiler de videos por cada mes, ordenados por fecha de alquiler
* Listar información de videos disponibles incluido el género

SE PIDE:

Diseño físico (para Oracle)
1.  Traducir modelo lógico a SGBD (Script DDL) --> Ya lo tienen !!
2.  Diseñar organización física para almacenamiento de los datos
2.1.  Realice el análisis transaccional e identifique cuales son las tablas críticas


# Trabajo Resuelto

# Propuesta de almacenamiento de datos
## Caso de estudio: Alquiler de videos
## Hardware: Data Storage de 24 Discos

## Nro de discos usados: 4 discos

## Distribución de discos:
	1 - Tabla Socio
	1 - Tablas Pelicula, Director, Participantes, Actor
	1 - Tabla Alquileres
	1 - Tabla Ejemplar

## Justificación:
Teniendo en cuenta que se puede tener un número elevado de películas se decidió poner la tabla Pelicula en un disco único, junto a las tablas de Director, Participantes y  Actor que complementan la información de la película.
