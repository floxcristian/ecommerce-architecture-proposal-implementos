# Comparativa de Herramientas CI/CD: GitHub Actions vs Google Cloud Build

Este documento presenta una comparación técnica entre dos plataformas de automatización de integración y despliegue continuo (CI/CD): **GitHub Actions (GHA)** y **Google Cloud Build (GCB)**. Ambas herramientas permiten automatizar flujos de trabajo de compilación, prueba y despliegue, pero tienen enfoques y fortalezas distintas.

## 🧪 Tabla Comparativa

| Característica                        | **GitHub Actions (GHA)**                 | **Google Cloud Build (GCB)**                       |
| ------------------------------------- | ---------------------------------------- | -------------------------------------------------- |
| **Proveedor**                         | GitHub (Microsoft)                       | Google Cloud Platform                              |
| **Integración con GitHub**            | ✅ Nativa y total                        | ⚠️ Parcial (requiere configurar triggers)          |
| **Soporte para repos privados**       | ✅ Incluido en todos los planes          | ✅ Sí, con permisos de acceso                      |
| **Configuración**                     | ✅ YAML en `.github/workflows/`          | ✅ YAML en `cloudbuild.yaml`                       |
| **Facilidad de uso**                  | ✅ Muy intuitivo                         | ⚠️ Mayor curva de aprendizaje                      |
| **Ejecutores personalizados**         | ✅ Soporte (runners self-hosted)         | ⚠️ Limitado, orientado a infraestructura de Google |
| **Costo**                             | ✅ Gratuito con límites generosos        | ✅ Gratuito con límites (120 min/día)              |
| **Logs y monitoreo**                  | ✅ Consola integrada en GitHub           | ✅ Stackdriver / Cloud Logging                     |
| **Integración con GCP**               | ⚠️ Requiere configuración adicional      | ✅ Nativa y profunda                               |
| **Escalabilidad automática**          | ✅ Soporte cloud                         | ✅ Escalado gestionado por GCB                     |
| **Marketplace de acciones**           | ✅ Amplio y activo                       | ❌ No aplica                                       |
| **Despliegues automáticos**           | ✅ Fácil integración con cualquier cloud | ✅ Optimizado para GCP                             |
| **Control de versiones de pipelines** | ✅ Versionado con el código fuente       | ✅ También versionado en el repositorio            |

---

## 🏆 Recomendación: **GitHub Actions**

**¿Por qué GitHub Actions?**

- ✅ Integración total con GitHub sin necesidad de configurar otros servicios externos.
- ✅ Flujo de trabajo sencillo y transparente a través de YAML versionado.
- ✅ Gran ecosistema gracias al **GitHub Actions Marketplace**, con acciones reutilizables.
- ✅ Ideal para proyectos multi-cloud o repositorios que ya viven en GitHub.
- ✅ Gratis con generosos límites para proyectos pequeños y medianos.

GitHub Actions es una solución **más universal, fácil de adoptar y flexible**, especialmente si tu código ya está en GitHub y trabajas con múltiples servicios cloud.

---

## 📝 ¿Cuándo usar cada uno?

- **GitHub Actions (GHA)**: Ideal para desarrolladores que ya usan GitHub, buscan rapidez en la configuración y flexibilidad multi-cloud.
- **Google Cloud Build (GCB)**: Recomendado si toda tu infraestructura ya está en **Google Cloud** y buscas una solución altamente integrada con servicios como Cloud Run, App Engine o GKE.

---

¿Quieres que agregue un ejemplo real de workflow para cada herramienta o integrar esta comparación en un README general de arquitectura?
