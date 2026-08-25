# Evidencias de Active Directory

Esta sección contiene las evidencias relacionadas con la instalación,
configuración y administración de Active Directory Domain Services (AD DS)
en el servidor `SRV-DC01`.

## Servidor

- **Hostname:** `SRV-DC01`
- **Sistema operativo:** Windows Server 2019
- **Dirección IPv4:** `192.168.10.10`
- **Red:** `192.168.10.0/24`

## Evidencias

| Archivo | Descripción |
|---|---|
| `08-add-ad-ds-role.png` | Asistente de Windows Server preparado para instalar el rol Servicios de dominio de Active Directory |

## Objetivos

La infraestructura de Active Directory tendrá como objetivos:

- Crear un dominio para el laboratorio.
- Configurar `SRV-DC01` como controlador de dominio.
- Proporcionar DNS mediante Active Directory.
- Crear una estructura de Unidades Organizativas (OU).
- Crear usuarios y grupos.
- Aplicar Directivas de Grupo (GPO).
- Integrar posteriormente equipos cliente Windows en el dominio.

## Seguridad

Las capturas y documentación no deben contener:

- Contraseñas.
- Claves de producto.
- Tokens o credenciales.
- Información personal real.
- Otros secretos de configuración.

Las cuentas y credenciales utilizadas en el laboratorio serán exclusivamente
de prueba.
