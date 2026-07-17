<div align="center">

# Johnny Rondón

**Ingeniero en Informática · Full Stack con orientación al Backend**

[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:johnnyarondonp@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/johnny-rond%C3%B3n-9064962b8/)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://johnny-portfolio-os.vercel.app)

</div>

---

Desarrollador Full Stack especializado en Laravel y React. Construyo sistemas desde la arquitectura de la base de datos hasta la interfaz, priorizando la integridad de los datos, el control de concurrencia y una lógica de negocio precisa. Mi objetivo es escribir código predecible, altamente mantenible y estructurado para resolver problemas en producción.

---

### Stack

**Backend**
PHP 8.3+ · Laravel 13 · PostgreSQL · MySQL · SQLite · RESTful APIs · Redis

**Frontend**
React 19 · TypeScript · Inertia.js · Alpine.js · Tailwind CSS · Framer Motion

**UI & Componentes**
shadcn/ui · Radix UI · Recharts · Lucide Icons

**Herramientas**
Vite · Git · PHPUnit · React Hook Form · Zustand

---

### Experiencia y Casos de Éxito Freelance
*Desarrollo de Software Independiente — Enfoque en Backend, Rendimiento & Infraestructura (2025 - Presente)*

Trabajo con clientes bajo estrictos acuerdos de confidencialidad (NDA), rescatando, optimizando y escalando plataformas en producción con desafíos críticos de concurrencia, seguridad y arquitectura.

#### 💬 Arquitectura en Tiempo Real y Alta Concurrencia
*   **Seguridad & Validación:** Identificación y mitigación de una vulnerabilidad crítica de omisión de autenticación (bypass de contraseña) en paneles administrativos y reestructuración de queries lógicas que exponían registros comprometidos.
*   **Optimización de Base de Datos:** Eliminación de más de 100 constraints duplicados e implementación de índices compuestos en PostgreSQL, acelerando consultas complejas de chat entre **5x y 10x**.
*   **Estrategias de Caché:** Integración de capas de persistencia con Redis para mitigar el cuello de botella en la base de datos, reduciendo en un **80%** las lecturas directas por petición.
*   **Escalabilidad Vertical:** Migración de backend de proceso único a un clúster de producción con PM2 y adaptador Redis para Socket.IO, incrementando masivamente el límite de concurrencia de usuarios simultáneos.
*   **Pruebas de Estrés:** Diseño y ejecución de suites de pruebas automatizadas con **k6**, simulando cargas intensas de hasta **1,000 usuarios virtuales concurrentes** para garantizar la estabilidad del servicio.

#### 📱 Optimización de Plataformas Sociales y Feeds Dinámicos
*   **Resolución de Cuellos de Botella:** Diagnóstico y corrección del problema de consultas N+1 en feeds principales mediante carga diferida previa (Eager Loading), reduciendo de **~300 a 0 las queries redundantes** por petición.
*   **Procesamiento Asíncrono:** Delegación de tareas pesadas de notificación masiva hacia Jobs procesados en background mediante colas (Queues), optimizando el tiempo de respuesta inmediato de la API rest.
*   **Ciclo de Vida de Datos:** Implementación de políticas de invalidación automática de caché para interacciones en tiempo real de alta frecuencia (estados, likes y suscripciones).

#### 🏢 Infraestructura y Sistemas Corporativos
*   **Web Performance Optimization (WPO):** Reestructuración de consultas pesadas y renderizado en Next.js, logrando disminuir tiempos de carga iniciales críticos de **~40 segundos** a rangos óptimos de respuesta.
*   **Single Sign-On (SSO):** Diseño e integración de flujos unificados de inicio de sesión social (Google/Facebook) para compartir ecosistemas de autenticación entre múltiples plataformas independientes.
*   **Sysadmin & DevOps:** Gestión de despliegues directos a producción en servidores VPS Linux (Ubuntu vía SSH) con configuración de políticas de respaldos automatizados y estrategias ágiles de rollback.

---

### Proyectos Personales

#### [Zoion — Gestión Veterinaria](https://github.com/johnnyarondonp-web/Zoion-sistema)
Plataforma ERP para clínicas veterinarias con RBAC multinivel y booking en tiempo real.

- Asignación de médicos por Round-Robin basada en carga diaria
- Bloqueos atómicos con `Cache::lock` para prevenir race conditions en reservas concurrentes
- Validación de unicidad global (cédula, teléfono, email) para evitar colisiones entre roles
- Suite de tests con PHPUnit sobre SQLite en memoria cubriendo autenticación, Walk-in y permisos

**Stack:** Laravel 13 · React 19 · TypeScript · Inertia.js · PostgreSQL · Redis

---

#### [Eunoia — Inventario y POS](https://github.com/johnnyarondonp-web/eunoia-sistema)
Sistema de punto de venta con lógica contable FIFO y soporte multi-moneda en tiempo real.

- Inventario por lotes FIFO con trazabilidad de costos por `SaleItem`
- Cálculo de ganancia  por venta comparando precio de venta contra costo exacto del lote
- Integración con API del BCV (tasa automática cada 30 min con fallback manual)
- Transacciones atómicas en ventas y cancelaciones con restauración exacta de lotes

**Stack:** Laravel 13 · Blade · Alpine.js · Tailwind CSS · MySQL

---

#### [Portfolio OS](https://github.com/johnnyarondonp-web/Portfolio-os)
Portafolio personal construido como un escritorio web interactivo con gestor de ventanas, múltiples temas y secuencia de arranque.

**Stack:** React 19 · Vite · Tailwind CSS v4 · Framer Motion
