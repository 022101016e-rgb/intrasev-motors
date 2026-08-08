# Intrasev Motors — Oficina

Sistema interno de gestión para la oficina de **Intrasev Motors**. Aplicación web ligera (un solo archivo HTML) que corre directamente en el navegador y guarda los datos localmente en el dispositivo.

## 🚗 Módulos

| Módulo | Descripción |
| ------ | ----------- |
| 🚗 **CLM 2000** | Control de ventas y productos. Registro de ventas, canjes de unidades gratis (1 por cada 6 vendidos), inventario y alertas de stock. |
| 💰 **Finanzas** | Resumen de ventas por día, semana y mes, con historial de movimientos y búsqueda por cliente. |

## ✨ Características

- 💾 **Sin servidor ni base de datos**: los datos se almacenan con `localStorage` del navegador.
- 📱 **Responsivo**: diseño adaptable para uso desde el celular o la computadora.
- 🔍 **Búsqueda en tiempo real** en productos y finanzas.
- 🎁 **Promoción automática**: control de unidades gratis (1 por cada 6 CLM 2000 vendidos).
- 📦 **Alertas de stock**: estados visuales para stock agotado, bajo u óptimo.

## 🛠️ Requisitos

- Navegador web moderno (Chrome, Firefox, Edge, Safari).
- No requiere instalación de dependencias ni servidor.

## 🚀 Uso

1. Abre el archivo `src/index.html` directamente en el navegador (doble clic), o
2. Sírvelo con cualquier servidor estático:

```bash
python3 -m http.server 8080
```

Luego visita `http://localhost:8080`.

## 📁 Estructura

```
intrasev-motors/
├── docs/           # Documentación del proyecto
├── src/            # Código fuente
│   └── index.html  # Aplicación completa (HTML + CSS + JS)
├── README.md
└── .gitignore
```

## ℹ️ Nota

Los datos se guardan únicamente en el navegador donde se usa la aplicación (`localStorage`). No hay persistencia en servidor ni sincronización entre dispositivos.
