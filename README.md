# 🔑 Proyecto QR - Páginas para Llaves Perdidas

Este proyecto fue desarrollado con **Astro** y permite generar una página única para cada familia, vinculada a un **QR impreso en llaveros**. Al escanear el código QR, se accede a una página que muestra los números de contacto de esa familia.

## ✨ Características

- ✅ Página por familia generada desde un JSON
- ✅ Rutas dinámicas como `/familia/1`, `/familia/2`, etc.
- ✅ Estilo moderno y responsivo
- ✅ Teléfonos clickeables (`tel:`) para llamar directamente desde el celular
- ✅ Animaciones suaves y fondo con gradiente

## 📁 Estructura del Proyecto
astro-llaves/
├── public/
├── src/
│ ├── data/
│ │ └── familias.json
│ └── pages/
│ └── familia/
│ └── [id].astro
│ └── index.astro (opcional)
├── package.json
├── astro.config.mjs
└── README.md


## 📄 Archivo `familias.json`

```json
[
  {
    "id": "1",
    "nombre": "Familia Gómez",
    "telefono": "1122334455",
    "alternativos": ["1166778899", "1144556677"]
  },
  {
    "id": "2",
    "nombre": "Familia Pérez",
    "telefono": "1199887766",
    "alternativos": ["1100110011"]
  }
]
