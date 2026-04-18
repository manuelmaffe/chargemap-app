# Voltio ⚡

Mapa interactivo de estaciones de carga para vehículos eléctricos con sistema de reservas y billetera virtual.

## Features

- 🗺️ Mapa interactivo con estaciones de carga reales (OpenStreetMap + Overpass API)
- 🔍 Búsqueda de direcciones (Nominatim)
- 📊 Ocupación en tiempo real por estación (simulada)
- 📅 Sistema de reservas de puntos de carga
- 💰 Billetera virtual con carga de crédito y historial de transacciones
- 🔐 Login/logout con persistencia en sesión
- 📍 Geolocalización del usuario
- 🌙 Dark mode

## Stack

- **Frontend:** HTML, CSS, JavaScript (vanilla)
- **Mapa:** Leaflet + OpenStreetMap tiles
- **Datos:** Overpass API (estaciones de carga de OSM)
- **Geocoding:** Nominatim (OpenStreetMap)
- **Deploy:** Vercel (static)

## Deploy en Vercel

```bash
# Con Vercel CLI
npm i -g vercel
vercel

# O con Claude Code
claude "deploy this to vercel"
```

También podés conectar el repo a Vercel desde el dashboard y hace deploy automático en cada push.

## Desarrollo local

```bash
npx serve public -l 3000
# Abrir http://localhost:3000
```

## Notas

- No requiere API keys — todo usa servicios abiertos y gratuitos
- La autenticación, reservas, billetera y ocupación son simuladas en el frontend (sessionStorage)
- Para producción real se necesitaría un backend con base de datos
