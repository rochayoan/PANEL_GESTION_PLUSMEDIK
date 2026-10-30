# PANEL_GESTION_PLUSMEDIK

Sistema independiente de cuentas y autenticación para personal y pacientes de Plusmedik.

## Estado
**En desarrollo. No apto para producción.** El código acumulado de las fases 1–8 todavía debe auditarse, compilarse e integrarse. Este repositorio no contiene por ahora la aplicación completa.

## Alcance previsto
- Acceso unificado para personal y pacientes.
- Cuentas creadas exclusivamente por invitación.
- Activación y recuperación de contraseña por correo.
- Sesiones seguras y autorización por roles.
- Backend NestJS, frontend Next.js y PostgreSQL.
- Preparación para VPS propia, sin despliegue.

## Seguridad
Repositorio público: **no subir** contraseñas, tokens, archivos .env, datos de pacientes, credenciales SMTP, volcados de base de datos ni claves privadas.

## Colaboración
El desarrollo se realizará en una rama de trabajo; los cambios a main deben revisarse mediante pull requests.

## Pendientes
- Incorporar y auditar el código acumulado de las fases 1–8.
- Verificar compilación, migraciones y pruebas.
- Completar correo transaccional y controles de seguridad.
- Validar el sistema antes de desplegar.

No hay servicios reales configurados ni despliegues autorizados.
