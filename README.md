# Mi-Ruta-Financiera
Herramienta que permite administrar, trazar mis finanzas y proyectar tiempos estimados en cubrir compromisos financieros
# Mi Ruta Financiera

Sistema personal para gestionar deudas ("frentes"), proyectar pagos y alcanzar metas financieras.  
Diseñado para ser simple, visual y fácil de usar desde el navegador.

## 🚀 Características

- **Gestión de frentes** (acreedores): nombre, tipo, saldo, aporte mensual, prioridad.
- **Cálculos automáticos**: saldo restante, porcentaje pagado, tiempo estimado de liquidación.
- **Importación desde CSV** (copiar/pegar desde Google Sheets u otras hojas).
- **Exportación a CSV** para respaldo o análisis externo.
- **Simulador**: ajusta tu aporte mensual y mira cómo se reduce el tiempo de deuda.
- **Calendario de pagos**: proyección mes a mes del progreso.
- **Metas personales**: define objetivos financieros (viajes, fondo de emergencia, etc.) y sigue su avance.
- **Historial de abonos**: registra cada pago y reviértelo si es necesario.
- **Persistencia local**: los datos se guardan automáticamente en tu navegador.

## 🛠️ Tecnologías

- Vue.js 2 (sin build, CDN)
- Tailwind CSS
- Chart.js (gráficos)
- Lucide (iconos)
- PapaParse (parseo de CSV)

## 📦 Cómo usarlo

1. Descarga el archivo `index.html` (o clona el repositorio).
2. Ábrelo en cualquier navegador moderno (no requiere servidor).
3. Agrega tus frentes manualmente o impórtalos desde un CSV.
4. Registra tus pagos periódicamente y observa cómo avanza tu plan.

## 🔜 Próximos pasos (Opción 3)

Este código es la base para la integración con **Google Sheets API**, que permitirá:
- Sincronización automática con tu hoja de cálculo.
- Lectura y escritura directa desde Google Sheets.
- Mantener tu hoja como fuente de verdad central.

## 📄 Licencia

MIT

---

**Autor:** Aurelio Robles  
**Fecha:** Marzo 2026
