# Estado de entrega — Plusmedik Auth (fases 1–8)

## Objetivo
Módulo independiente de autenticación para personal y pacientes de Plusmedik. Login unificado, cuentas por invitación, recuperación de contraseñas por correo, sesiones y permisos.

## Arquitectura prevista
- Frontend: Next.js / TypeScript.
- Backend: NestJS / TypeScript.
- Base de datos: PostgreSQL / Prisma.
- Contraseñas: Argon2id.
- Hosting futuro: VPS propia con Docker.
- Repositorio público: nunca incluir secretos ni datos personales.

## Código preparado fuera de GitHub
El paquete acumulativo de la Fase 8 consta de 68 archivos (ZIP disponible en la conversación de ChatGPT). Incluye:
- apps/api: servicios y controladores de autenticación.
- apps/web: formularios y páginas Next.js.
- prisma/schema.prisma: modelo inicial de datos.
- packages/contracts: tipos compartidos.
- docs: arquitectura, seguridad y avances de fases.
- infra: plantilla PostgreSQL Docker Compose y ejemplos de configuración.

**ATENCIÓN: este documento NO significa que los 68 archivos estén subidos a GitHub.**

## Bloqueos para producción
1. Falta verificar instalación limpia, compilación y pruebas.
2. Falta correo transaccional real y entrega verificable.
3. Falta bootstrap seguro del primer ADMIN.
4. Falta rate limiting persistente y revisión CSRF.
5. Faltan migraciones Prisma validadas y pruebas de concurrencia.
6. Faltan Dockerfiles de frontend/backend y proxy HTTPS.
7. Falta CI y validación E2E.

## Criterio de entrega
No desplegar ni usar cuentas reales hasta completar las pruebas y la revisión de seguridad.

## Colaboración
Trabajar en `develop` y proponer cambios a `main` mediante pull requests.
