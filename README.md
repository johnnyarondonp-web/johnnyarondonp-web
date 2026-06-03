<div align="center">

# Johnny Rondón

**Ingeniero en Informática · Full Stack con orientación al Backend**

[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:johnnyarondonp@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/johnny-rond%C3%B3n-9064962b8/)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://johnny-portfolio-os.vercel.app)

</div>

---

Desarrollador Full Stack especializado en Laravel y React. Construyo sistemas desde la arquitectura de base de datos hasta la interfaz — con foco en integridad de datos, control de concurrencia y lógica de negocio precisa. Me importa que el código sea predecible, mantenible y correcto antes que impresionante.

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

### Proyectos

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
- Cálculo de ganancia real por venta comparando precio de venta contra costo exacto del lote
- Integración con API del BCV (tasa automática cada 30 min con fallback manual)
- Transacciones atómicas en ventas y cancelaciones con restauración exacta de lotes

**Stack:** Laravel 13 · Blade · Alpine.js · Tailwind CSS · MySQL

---

#### [Portfolio OS](https://github.com/johnnyarondonp-web/Portfolio-os)
Portafolio personal construido como un escritorio web interactivo con gestor de ventanas, múltiples temas y secuencia de arranque.

**Stack:** React 19 · Vite · Tailwind CSS v4 · Framer Motion
