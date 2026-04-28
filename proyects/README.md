# Active Directory Security Assessment

## Resumen

Evaluación de seguridad en un entorno Active Directory simulado, donde se logró comprometer completamente el dominio mediante una cadena de explotación que abarca desde acceso inicial no autenticado hasta persistencia avanzada.

El ataque se basó en la explotación encadenada de múltiples vulnerabilidades, incluyendo servicios mal configurados, exposición de credenciales y debilidades en la gestión de privilegios.

## Objetivo

Obtener acceso a un usuario con privilegios elevados en el controlador de dominio mediante técnicas de pentesting en un entorno segmentado.

## Entorno

- Kali Linux (atacante)
- Linux User (pivot)
- Windows User
- Windows Domain Controller

Infraestructura segmentada con múltiples redes internas.

## Metodología

- Reconocimiento y enumeración (Nmap)
- Explotación inicial (FTP + Web RCE)
- Escalada de privilegios
- Pivoting y tunneling (SSH)
- Movimiento lateral
- Enumeración de Active Directory
- Explotación de Kerberos (Kerberoasting)
- Compromiso del dominio

## Cadena de ataque

1. Acceso FTP anónimo
2. Subida de reverse shell (RCE)
3. Acceso inicial como www-data
4. Obtención de credenciales en texto claro
5. Crackeo de hash MD5 (usuario shrek)
6. Acceso SSH y pivoting entre redes
7. Túneles SOCKS para acceso a red interna
8. Acceso a máquina Windows vía RDP
9. Enumeración de Active Directory
10. Ataque Kerberoasting sobre cuentas de servicio
11. Crackeo de credenciales (iis_service)
12. Acceso al Domain Controller
13. Dump de credenciales (NTDS.dit)
14. Compromiso de cuenta krbtgt (Golden Ticket)

## Vulnerabilidades clave

- FTP anónimo habilitado
- Ejecución remota de código (RCE)
- Credenciales expuestas en texto claro
- Uso de hash débil (MD5)
- Segmentación de red insuficiente
- Cuentas vulnerables a Kerberoasting
- Privilegios excesivos (Domain Admin)
- Exposición de NTDS.dit

## Impacto

Compromiso total del dominio Active Directory, incluyendo:
- Acceso a todos los usuarios
- Extracción de hashes
- Persistencia mediante Golden Ticket

## Recomendaciones

- Eliminación de accesos anónimos
- Validación de subida de archivos
- Gestión segura de credenciales
- Segmentación de red
- Principio de mínimo privilegio
- Protección de cuentas de servicio
- Monitorización de eventos de autenticación

## Informe completo

[Ver informe técnico](assets/active-directory-security-assessment.pdf)

## Nota

Laboratorio realizado en entorno controlado con fines educativos.
