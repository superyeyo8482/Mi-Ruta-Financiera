# Mi Ruta Financiera – Dashboard Inteligente de Compromisos y Efectivo

Aplicación web para gestionar deudas ("compromisos"), controlar el flujo de efectivo diario y recibir asistencia inteligente para distribuir ingresos extra.  
**Datos siempre locales** (en tu navegador) – no se comparte información con ningún servidor.

## 🚀 Demo en vivo

👉 [https://mi-ruta-financiera.vercel.app/](https://mi-ruta-financiera.vercel.app/)

## ✨ Características principales

### 📋 Gestión de compromisos (deudas o pagos programados)
- Crear, editar, eliminar compromisos.
- Registrar **abonos** (pagos) y **cargos** (nuevas deudas).
- Cada compromiso muestra: saldo restante, aportación mensual, total abonado, progreso visual y fecha de vencimiento opcional.
- **Exportar reporte individual en CSV** – ideal para enviar por WhatsApp o correo a los acreedores o para tu control personal.
- Exportar todos los compromisos a un solo archivo CSV.

### 💰 Flujo de efectivo
- Registrar ingresos y gastos diarios.
- Saldo disponible actualizado automáticamente.
- **Gráfico de evolución del saldo** en los últimos 30 días.
- Resumen del mes: total ingresos, gastos y flujo neto.
- Historial completo de movimientos con opción de eliminar.
- Exportar movimientos a CSV.

### 🧠 Asistente y prioridades
- **Asistente de distribución de ingresos extra**: ingresa un monto extra y el sistema te sugerirá cómo repartirlo entre tus compromisos, basado en:
  - **Prioridad máxima** (⭐) que tú defines (solo un compromiso puede tenerla).
  - **Prioridad normal** (alta, media, baja) para el resto.
- **Configuración de prioridades** visual: marca qué compromiso es tu prioridad máxima y ajusta la prioridad de cada uno.
- Sugerencia calculada con reglas simples (50% para prioridad máxima, el resto ponderado por nivel de prioridad). Puedes aplicar la distribución con un clic.

### 🔔 Notificaciones (opcionales)
- El navegador pedirá permiso al cargar la página.
- Recordatorio cuando un compromiso está próximo a vencer (3 días, 1 día o el mismo día).
- Resumen semanal del total abonado en la última semana.

### 📥 Importación/exportación
- Importar compromisos desde CSV (formato esperado: `nombre,tipo,saldo_total,saldo_pagado,aporte_mensual,prioridad`).
- Exportar todos los datos (compromisos o movimientos de efectivo) a CSV.

## 🛠️ Tecnologías utilizadas

- **Vue.js 2** (CDN) – reactividad sin necesidad de compilación.
- **Tailwind CSS** – estilos responsivos.
- **Chart.js** – gráfico de evolución del efectivo.
- **Lucide** – iconos modernos.
- **PapaParse** – parseo de CSV.

## 📦 Instalación y despliegue

1. **Descarga o clona** este repositorio.
2. Abre el archivo `index.html` en tu navegador (funciona sin servidor).
3. Para desplegar en **Vercel**:
   - Arrastra la carpeta del proyecto a [vercel.com](https://vercel.com) o conecta tu repositorio de GitHub.
   - El despliegue es automático.

## 📖 Cómo usar la importación de CSV

El sistema espera un CSV con **encabezados exactos**:

```csv
nombre,tipo,saldo_total,saldo_pagado,aporte_mensual,prioridad
Préstamo familiar,Familiar,50000,10000,5000,alta
Tarjeta BBVA,Tarjeta de Crédito,15000,0,3000,media


---

## 📌 **Archivo LICENSE (opcional, pero recomendado)**

Si deseas incluir la licencia MIT, crea un archivo `LICENSE` con este contenido:

```text
MIT License

Copyright (c) 2026 Aurelio Robles

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.