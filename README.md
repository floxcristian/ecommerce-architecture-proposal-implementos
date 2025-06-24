# 🛍️ Guía Profesional de Ecommerce con Microservicios

Una guía completa para desarrollar y desplegar ecommerce escalable usando tecnologías modernas, microservicios y mejores prácticas tanto para desarrollo como producción.

## 🎯 Alcance de la Guía

Esta guía cubre desde la optimización frontend hasta la infraestructura completa:

- **Frontend**: Angular con optimizaciones avanzadas
- **Backend**: Microservicios con NestJS
- **Infraestructura**: Kubernetes, Docker, CI/CD
- **Observabilidad**: Monitoring, logging y trazas
- **Seguridad**: TLS, autenticación y mejores prácticas

## 🧩 Stack Tecnológico

| Área                | Tecnologías                                         |
| ------------------- | --------------------------------------------------- |
| **Frontend**        | NX Monorepo + Angular                               |
| **Backend**         | NX + NestJS + Microservicios + BullMQ               |
| **Infraestructura** | GCP (prod) + On Premise (dev) + Kubernetes + Docker |
| **Orquestación**    | Traefik + cert-manager + Let's Encrypt              |
| **CI/CD**           | GitHub Actions + Helm + Docker Registry             |
| **Observabilidad**  | Prometheus + Grafana + Loki + Jaeger                |

## 📋 Subdominios y Arquitectura

### Desarrollo

- `dev.implementos.cl` - Frontend principal
- `admin.dev.implementos.cl` - Panel administrativo
- `api.dev.implementos.cl` - API Gateway
- `traefik.dev.implementos.cl` - Dashboard Traefik

### Producción

- `implementos.cl` - Frontend principal
- `admin.implementos.cl` - Panel administrativo
- `api.implementos.cl` - API Gateway
- `traefik.implementos.cl` - Dashboard Traefik

> 🌥️ Todos los subdominios pasan por Cloudflare con WAF, caché, y protección DDoS activados.
