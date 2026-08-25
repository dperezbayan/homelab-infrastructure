# 01 - Planificación de la infraestructura

## Objetivo

Diseñar e implementar un laboratorio de infraestructura IT virtualizada
que simule el entorno tecnológico de una pequeña empresa.

El laboratorio permitirá practicar administración de sistemas Windows y Linux,
servicios de red, gestión de usuarios, monitorización, copias de seguridad,
automatización y seguridad.

## Virtualización

La infraestructura se implementará mediante máquinas virtuales utilizando
Oracle VirtualBox.

## Máquinas virtuales

### SRV-DC01

Servidor principal de infraestructura.

Funciones previstas:

- Active Directory Domain Services
- DNS
- DHCP
- Gestión de usuarios y grupos
- Directivas de grupo (GPO)

### SRV-LNX01

Servidor Linux.

Funciones previstas:

- SSH
- Servidor web
- Base de datos
- Automatización mediante Bash
- Servicios adicionales según las necesidades del laboratorio

### CLI-WIN01

Equipo cliente Windows.

Funciones previstas:

- Unión al dominio
- Aplicación de GPO
- Pruebas de autenticación
- Acceso a recursos compartidos
- Comprobación de servicios de red

## Red

Se utilizará una red virtual privada para comunicar las máquinas del
laboratorio.

La configuración definitiva de direccionamiento IP se documentará antes
de comenzar la instalación.

## Evolución del laboratorio

El laboratorio se ampliará progresivamente con:

- Monitorización
- Copias de seguridad
- Automatización
- Seguridad
- Resolución de incidencias
- Documentación técnica

## Estado

🟡 Planificación
