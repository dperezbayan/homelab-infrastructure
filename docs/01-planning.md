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
