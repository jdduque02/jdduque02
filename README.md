<div align="center">

# Jose David Duque Gutiérrez

**Desarrollador Senior Backend** · Arquitectura de Microservicios · Node.js & Python

Medellín, Colombia · Remote

[LinkedIn](https://linkedin.com/in/jose-david-duque-gutierrez-b504b51a1/) · [Email](mailto:jdduquegutierrez02@gmail.com) · [GitHub](https://github.com/jdduque02)

</div>

---

## Sobre mí

Más de 6 años diseñando e implementando arquitecturas de microservicios escalables. Trabajo principalmente con **NestJS**, **FastAPI** y arquitectura **Hexagonal** (Controller → Service → Repository → Entity), con foco en Clean Code, SOLID y DRY.

Mi especialidad son los **servicios asíncronos**: cargas masivas de datos, procesamiento de archivos con colas de trabajo, eventos y reintentos automáticos — sistemas que se mantienen correctos y observables bajo carga real, no solo en el happy path.

Actualmente lidero la modernización de sistemas y la mentoría técnica de equipos bajo metodologías ágiles, con pipelines CI/CD en Jenkins y despliegue en GCP/AWS.

## Ahora mismo

- Construyendo **Cost Manager**, un sistema de gestión financiera personal end-to-end con arquitectura hexagonal.
- Profundizando en Kubernetes y arquitectura orientada a eventos.
- Abierto a colaborar en proyectos open source de backend en Node.js o Python.

---

## En números

6+ años en producción, 4 organizaciones, +3.380 líneas y 123 archivos entregados en microservicios de producción — desde plataformas financieras multi-tenant hasta pipelines de datos a escala.

| Rol | Organización | Periodo | Archivos | Líneas |
| --- | --- | --- | --- | --- |
| Desarrollador Senior Backend | Domina SAS | Abr 2025 – actualidad | 42 | +1.240 / −180 |
| Desarrollador Full Stack | DI – Data Innovations S.A.S | May 2022 – Abr 2025 | 38 | +980 / −310 |
| Desarrollador Web | DATA IN SITU S.A.S | Feb 2020 – Abr 2022 | 29 | +740 / −190 |
| Analista de Datos | Pintuco S.A.S | Jul 2019 – Ene 2020 | 14 | +420 / −80 |

---

## Proyecto destacado — Cost Manager

Sistema de gestión financiera personal end-to-end sobre arquitectura en 4 capas (Controller → Service → Repository → Entity), diseñado para escalar como microservicios.

```
Controller (HTTP) → Service (reglas de negocio) → Repository (persistencia) → Entity (Modelo)
                          ↑ dominio aislado de la infraestructura (Hexagonal)
```

| Repositorio | Descripción | Stack |
| --- | --- | --- |
| [api-cost-manager](https://github.com/jdduque02/api-cost-manager) | API multi-módulo: auth con Keycloak, cache Redis, mensajería RabbitMQ, procesamiento asíncrono, notificaciones WebSocket, i18n y auditoría. Documentada con Swagger, cubierta con Jest y SonarQube. | NestJS 11 · TypeScript · PostgreSQL/TypeORM · Redis · RabbitMQ · Keycloak |
| [cost-manager-web](https://github.com/jdduque02/cost-manager-web) | Panel web de costos, transacciones y objetivos financieros, sincronizado en tiempo real vía Socket.io. | React 19 · TanStack Query/Start · Tailwind CSS · shadcn/ui |
| [cost-manager-app-movil](https://github.com/jdduque02/cost-manager-app-movil) | App móvil para gestión de costos desde cualquier lugar. | React Native · Expo · TypeScript |

**Servicios asíncronos** — el flujo detrás de las cargas masivas y el procesamiento de archivos:

```
Cliente / Scheduler → Cola (RabbitMQ / Redis) → Worker → Persistencia → Notificación
    Sube CSV/XLSX         Encola el trabajo         Procesa     DB      WebSocket / Email
```

Con reintentos automáticos y dead-letter queues para trazabilidad, y seguimiento de estado por job: `pendiente → procesando → completado / fallido`.

---

## Stack principal

**Backend** — NestJS 11 · Node.js · TypeScript · FastAPI · Python · Express.js · Socket.io · JWT · Swagger

**Datos & mensajería** — PostgreSQL · TypeORM · Redis · MongoDB · MySQL · Keycloak · RabbitMQ

**DevOps & cloud** — Docker · Jenkins · GCP · AWS · Kubernetes · SonarQube · Jest

**Frontend** — React · TanStack Query · Tailwind CSS · Vite · Expo · React Native · Vue.js

**Flujo con IA** — GitHub Copilot para autocompletado y tests; OpenCode en terminal para explorar código e implementar features.

---

## Flujo de trabajo — GitFlow + Conventional Commits

```
main ────────────────●─── release/v1.2.0 ──●───────
develop ──●──────────●─────────●────────────●───────
feature/* ──●────────●────── fix/* ...
hotfix/* ────────────────────────●──→ main + develop
```

| Rama | Propósito |
| --- | --- |
| `main` | Producción estable; solo recibe cambios vía `release/*` o `hotfix/*` |
| `develop` | Integración diaria; origen de todas las features |
| `feature/<tipo>-<descripcion>` | Trabajo nuevo (`feat-`, `fix-`, `refactor-`, `perf-`, ...) |
| `release/vX.Y.Z` | Preparación y estabilización de versión antes de llegar a `main` |
| `hotfix/<descripcion>` | Corrección urgente en producción (regresa a `main` y `develop`) |

Ramas: `tipo/descripcion-corta` (`feat/auth-keycloak`, `fix/paginacion-fecha`). Commits: `tipo(scope): descripcion` — `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `build`, `ci`, `chore`, `revert`.

---

<div align="center">

![Stats](https://github-readme-stats.vercel.app/api?username=jdduque02&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=false)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=jdduque02&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=false&layout=compact)

</div>

---

<div align="center">

¿Proyecto, idea, o quieres hablar de backend y arquitectura? [Escríbeme](mailto:jdduquegutierrez02@gmail.com) o conecta en [LinkedIn](https://linkedin.com/in/jose-david-duque-gutierrez-b504b51a1/).

</div>
