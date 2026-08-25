# Homelab - Infraestructura IT Empresarial

Laboratorio de infraestructura IT virtualizada diseñado para simular el entorno tecnológico de una pequeña empresa.

El proyecto tiene como objetivo poner en práctica conocimientos de administración de sistemas, redes, servidores, monitorización, seguridad y automatización.

## Objetivos

- Diseñar una infraestructura IT virtualizada.
- Implementar Windows Server y Active Directory.
- Configurar DNS y DHCP.
- Administrar usuarios, grupos y equipos.
- Aplicar políticas mediante GPO.
- Implementar un servidor Linux.
- Configurar servicios de red y aplicaciones.
- Implementar monitorización.
- Automatizar tareas administrativas.
- Implementar copias de seguridad.
- Documentar procedimientos y resolución de incidencias.

## Tecnologías

Actualmente en planificación:

- VirtualBox
- Windows Server
- Windows
- Linux
- Active Directory
- DNS
- DHCP
- PowerShell
- Bash
- Git
- GitHub

## Arquitectura

```mermaid
flowchart TB
    HOST["PC anfitrión<br>Windows"]
    NETWORK["Red Host-Only<br>192.168.10.0/24"]
    DC["SRV-DC01<br>192.168.10.10<br><br>Active Directory<br>DNS<br>DHCP"]
    LNX["SRV-LNX01<br>192.168.10.20<br><br>Linux Server"]
    CLI["CLI-WIN01<br>DHCP<br><br>Windows Client"]

    HOST --- NETWORK
    NETWORK --- DC
    NETWORK --- LNX
    NETWORK --- CLI
```

## Documentación

La documentación se incorporará progresivamente a medida que se implementen y validen los diferentes componentes de la infraestructura.

## Estado del proyecto

🟡 En desarrollo

## Autor

Daniel Pérez
