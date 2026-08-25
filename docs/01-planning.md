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

## Recursos del equipo anfitrión

- RAM: 16 GB DDR3
- CPU: Intel Core i7-5600U @ 2.60 GHz
- Núcleos: 2 físicos / 4 hilos
- Espacio libre disponible: aproximadamente 300 GB

## Asignación de recursos

| Máquina | RAM | CPU | Disco | Función |
|---|---:|---:|---:|---|
| SRV-DC01 | 4 GB | 2 vCPU | 60 GB | Windows Server, AD, DNS y DHCP |
| CLI-WIN01 | 4 GB | 2 vCPU | 60 GB | Cliente Windows |
| SRV-LNX01 | 2 GB | 1 vCPU | 30 GB | Ubuntu Server y servicios Linux |

La asignación se ha diseñado teniendo en cuenta las limitaciones de CPU
del equipo anfitrión y dejando recursos suficientes para el sistema
operativo principal.

## Red

## Diseño de red

El laboratorio utilizará una red privada virtualizada con direccionamiento
IPv4 basado en la red 192.168.10.0/24.

### Parámetros

- Red: 192.168.10.0/24
- Máscara: 255.255.255.0
- Gateway: 192.168.10.1
- Servidor DNS: 192.168.10.10

### Direccionamiento

| Máquina | IP | Configuración |
|---|---|---|
| SRV-DC01 | 192.168.10.10 | Estática |
| SRV-LNX01 | 192.168.10.20 | Estática |
| CLI-WIN01 | DHCP | Automática |

### Dominio

El dominio interno utilizado por el laboratorio será:

empresa.test

### Nombres de host

- SRV-DC01.empresa.test
- SRV-LNX01.empresa.test
- CLI-WIN01.empresa.test

### Servicios de red

SRV-DC01 proporcionará inicialmente:

- Active Directory Domain Services
- DNS
- DHCP

## Justificación del diseño

Se ha utilizado una red /24 para disponer de un rango sencillo de gestionar
durante el laboratorio y suficiente para el número de dispositivos previsto.

Las direcciones de los servidores se han definido de forma estática para
garantizar que los servicios de infraestructura sean siempre accesibles
desde la misma dirección IP.

El equipo cliente utilizará DHCP para simular el comportamiento habitual
de los equipos de usuario dentro de una red empresarial.

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
