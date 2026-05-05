# Mi Ruta Financiera – Control total de tus finanzas personales

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![Vue.js](https://img.shields.io/badge/Vue.js-2.x-4FC08D?logo=vue.js)](https://vuejs.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-38B2AC?logo=tailwind-css)](https://tailwindcss.com/)

**Mi Ruta Financiera** es una aplicación web progresiva que te permite gestionar tus deudas (frentes), ingresos, gastos, metas y presupuesto de forma privada, con una capa de gamificación que te mantiene motivado sin alterar tus datos reales.

👉 [Demo en Vercel](https://mi-ruta-financiera.vercel.app) (ejemplo – despliega el tuyo)

---

## ✨ Características principales

### 📌 Frentes (acreedores)
- Crear, editar, eliminar frentes con nombre, tipo, saldo total, pagado, aporte mensual y prioridad.
- Registrar **abonos** (pagos) y **cargos** (nuevas deudas).
- Historial completo con saldo acumulado, editable y eliminable.
- Exportar estado de cuenta a **PDF** (formato profesional) y **CSV**.
- Importar historial de pagos desde CSV (ideal para migrar desde Google Sheets).

### 💰 Flujo de efectivo
- Ingresos y gastos diarios, saldo actualizado en tiempo real.
- Gráfico de evolución del saldo (últimos 30 días).
- Resumen mensual: total ingresos, gastos y flujo neto.
- Exportar a CSV y PDF.

### 🎯 Metas / Proyectos
- Define objetivos financieros (viaje, fondo de emergencia, etc.).
- Registra abonos y visualiza el progreso con barra de porcentaje.
- Logro automático y confeti al alcanzar la meta.

### 📊 Presupuesto base
- Gastos fijos y variables con periodicidad (semanal, quincenal, mensual, bimestral, trimestral, anual).
- Normalización a monto mensual y comparación con ingresos del mes.
- Superávit/déficit y porcentaje de cobertura.
- Histórico de evolución de los últimos 6 meses (tabla y gráfico).

### 😊 Bienestar y gamificación (sin alterar datos reales)
- Registro diario de humor (😊, 😌, 😐, 😕, 😞, 😠) con nota opcional.
- Gráfico de evolución del estado de ánimo.
- Listado histórico de estados de ánimo (eliminable).
- Notas personales de salud/medicación con etiquetas e historial anual.
- Sistema de **XP** y **niveles**:
  - Cada logro (liquidar frente o alcanzar meta) → +100 XP.
  - Subir de nivel cada 500 XP.
  - Barra de progreso visible en KPIs.
- **Rincón de Celebración** con historial de logros.

### 🕹️ Easter egg (código secreto) – ¡solo diversión!
- **Secuencia**: 3 clics en el logo de la brújula → 2 clics en la tarjeta "Total Frentes" → 1 clic en el fondo de la página.
- **Recompensa**: +100 XP, confeti dorado y sonido *ding*. También desbloquea el **"Poder Oculto"** en la pestaña Bienestar.
- **Poder Oculto**: +1000 XP una vez al día (no afecta deudas reales).

### 🧠 Asistente de distribución de ingresos extra
- Simulador de pagos (no modifica los frentes reales).
- Sugiere distribución basada en prioridad máxima (50%) y prioridad normal (alta/media/baja).
- Genera una **orden de pago imprimible** con los datos bancarios de cada frente.

### 🎨 Personalización y seguridad
- Logo personalizable mediante URL.
- Cambio de color primario (tema).
- Autenticación por contraseña (guardada en localStorage). Cada navegador tiene datos independientes.

### 📁 Importación/Exportación
- Importar frentes desde CSV (cabeceras: nombre, tipo, saldo_total, saldo_pagado, aporte_mensual, prioridad, comentario, ultimo_pago).
- Importar historial de abonos de un frente (fecha, monto, concepto).
- Exportar todos los frentes a CSV.
- Exportar movimientos de efectivo a CSV.
- Exportar reporte de frentes a PDF (general y por frente).

---

## 🛠️ Tecnologías

- **Vue.js 2** – reactividad sin compilación.
- **Tailwind CSS** – estilos responsivos.
- **Chart.js** – gráficos de evolución.
- **Lucide** – iconos modernos.
- **PapaParse** – parseo de CSV.
- **jsPDF + html2canvas** – generación de PDFs.
- **canvas-confetti** – efectos visuales.

---

## 📦 Instalación y despliegue

### Local (pruebas)
1. Descarga el archivo `index.html`.
2. Haz doble clic para abrirlo en tu navegador (necesitas conexión a internet para cargar las CDNs la primera vez).
3. Crea tu contraseña y empieza a usar la aplicación.

### En Vercel (producción)
1. Ve a [vercel.com](https://vercel.com) e inicia sesión.
2. Arrastra la carpeta que contiene el `index.html` a la interfaz de Vercel (o conecta tu repositorio de GitHub).
3. Vercel generará una URL pública. Compártela o úsala en tu móvil.

> **Nota:** Los datos se guardan en `localStorage`. Cada dispositivo/navegador tiene sus propios datos independientes.

---

## 📥 Formato de CSV para importación

### Frentes
```csv
nombre,tipo,saldo_total,saldo_pagado,aporte_mensual,prioridad,comentario,ultimo_pago
Papás,Familiar,102044,0,5000,media,Comentario opcional,2025-04-01
BBVA,Tarjeta de Crédito,7862.52,0,2000,alta,,
Historial de abonos de un frente
csv
fecha,monto,concepto
2025-04-25,5000,Pago quincena
2025-05-10,3000,Abono extra
🔮 Hoja de ruta
Integración con Google Sheets API (sincronización en la nube, acceso multi‑dispositivo).

Versión para negocios (control de inventario, ventas online, reportes personalizados).

Modelo de monetización (open core, suscripción SaaS, personalizaciones white‑label).

Aplicación móvil (PWA o nativa con Capacitor).

🤝 Contribuciones
Las contribuciones son bienvenidas. Por favor, abre un issue o un pull request para discutir cambios importantes.

📄 Licencia
MIT © 2026 Aurelio Robles (ARP)

📧 Contacto
Autor: Aurelio Robles
GitHub: @aureliorobles
Correo: [aurelio@robles.ws]
Telefono: 5546539933
⭐ Si esta herramienta te ha sido útil, ¡considera darle una estrella en GitHub!
Desarrollada para tomar el control de tus finanzas de manera privada, divertida y eficiente.
