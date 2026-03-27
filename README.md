# GDG ICA Data

Datos estructurados de **GDG ICA** (Google Developer Group Ica). Fuente de verdad para la app Flutter y otros clientes.

## Estructura

```
events/
  index.json              # Lista resumida de todos los eventos
  devfest-2024.json       # Detalle completo de cada evento
  ...
speakers/
  index.json              # Lista resumida de todos los speakers
  eduardo-ormeno.json     # Perfil completo de cada speaker
  ...
about/
  team.json               # Equipo organizador + miembros
  stats.json              # Estadisticas de la comunidad
  partners.json           # Partners y sponsors
gallery/
  gallery.json            # Fotos de eventos
resources/
  learning-paths.json     # Rutas de aprendizaje
  codelabs.json           # Recursos curados
```

## Consumo

Los datos se sirven via `raw.githubusercontent.com`:

```
https://raw.githubusercontent.com/GDGXICA/gdg-ica-data/main/events/index.json
```

## Formato

- Fechas en ISO 8601: `2024-11-23T09:00:00`
- URLs de imagenes absolutas: `https://gdgxica.github.io/events/devfest-2024.webp`
- Campos en `snake_case`
- UTF-8 con caracteres especiales (tildes, ñ)

## Contribuir

1. Edita/crea el JSON correspondiente
2. Abre un Pull Request
3. El CI valida el formato
4. Un CODEOWNER aprueba y mergea
