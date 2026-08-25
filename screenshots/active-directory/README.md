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

### 08 — Instalación de Active Directory Domain Services

Asistente de Windows Server preparado para instalar el rol de Servicios de dominio de Active Directory (AD DS).

![Instalación de Active Directory Domain Services](08-add-ad-ds-role.png)
## Objetivos

La infraestructura de Active Directory tendrá como objetivos:

- Crear un dominio para el laboratorio.
- Configurar `SRV-DC01` como controlador de dominio.
- Proporcionar DNS mediante Active Directory.
- Crear una estructura de Unidades Organizativas (OU).
- Crear usuarios y grupos.
- Aplicar Directivas de Grupo (GPO).
- Integrar posteriormente equipos cliente Windows en el dominio.

## Estructura de Unidades Organizativas

El dominio `adlab.local` utiliza una estructura de Unidades Organizativas (OU)
para separar usuarios, equipos, servidores y grupos.

```text
adlab.local
├── Usuarios
│   ├── Administracion
│   ├── IT
│   └── Usuarios
├── Equipos
│   ├── PuestosTrabajo
│   └── Portatiles
├── Servidores
└── Grupos
```

## Grupos de seguridad

Se han creado grupos de seguridad para facilitar la administración de permisos
y la aplicación de políticas de grupo.

| Grupo | Tipo | Ámbito | Propósito |
|---|---|---|---|
| `IT-Admins` | Seguridad | Global | Administradores del área de TI |
| `GG-Usuarios` | Seguridad | Global | Usuarios estándar del dominio |
| `GG-Administracion` | Seguridad | Global | Usuarios del área de administración |

La utilización de grupos permite evitar asignar permisos individualmente a
cada usuario y facilita la administración de la infraestructura.

## Seguridad

Las capturas y documentación no deben contener:

- Contraseñas.
- Claves de producto.
- Tokens o credenciales.
- Información personal real.
- Otros secretos de configuración.

Las cuentas y credenciales utilizadas en el laboratorio serán exclusivamente
de prueba.
