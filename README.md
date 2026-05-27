Panel de control web para **Mihomo** (cliente proxy) con interfaz visual y actualización en tiempo real.

## Características

- 📊 **Dashboard en tiempo real** – Tráfico, conexiones activas y latencia.
- 🔌 **WebSocket con reconexión automática** – Estado actualizado sin recargar.
- 🧩 **Interfaz modular** – Componentes reutilizables y optimización del DOM.
- 📦 **PWA (Progressive Web App)** – Instalable y con soporte offline básico.
- 🔒 **Sanitización y validación** – Seguridad en la comunicación con la API.

## Estructura del proyecto
mihomo-gate/
├── index.html
├── css/
│   └── styles.css          # (Opcional) overrides y animaciones
├── js/
│   ├── core/
│   │   ├── state.js        # Store reactivo centralizado
│   │   ├── api.js          # Cliente HTTP Mihomo
│   │   └── ws.js           # Gestor de WebSocket con reconexión
│   ├── ui/
│   │   ├── renderer.js     # Actualizaciones DOM optimizadas
│   │   ├── components.js   # Componentes reutilizables
│   │   └── chart.js        # Gráfico de tráfico
│   ├── utils/
│   │   ├── format.js       # Utilidades (bytes, tiempo, latencia)
│   │   ├── debounce.js     # Control de frecuencia
│   │   └── security.js     # Sanitización y validación
│   └── main.js             # Inicialización y router
└── manifest.json           # PWA
