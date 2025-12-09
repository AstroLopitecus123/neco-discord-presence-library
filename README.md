# Neco Discord Presence - Biblioteca de Programas

Este repositorio contiene una biblioteca colaborativa de configuraciones de Discord Rich Presence para diferentes programas y aplicaciones.

## ¿Qué es esto?

Esta biblioteca permite a los usuarios de **Neco Discord Presence** compartir y descargar configuraciones predefinidas de programas populares, incluyendo:

- Configuración de Discord Rich Presence
- Imágenes personalizadas
- Detalles y estados personalizados
- Categorías

## Estructura

```
neco-discord-presence-library/
├── programs.json          # Lista principal de todos los programas disponibles
├── programs/              # Archivos JSON individuales de cada programa
│   └── program-*.json
├── images/                # Imágenes de los programas
│   └── program-*-image.png
└── README.md             # Este archivo
```

## Formato de un programa

Cada programa en `programs/` tiene el siguiente formato:

```json
{
  "name": "Nombre del Programa",
  "applicationId": "TU_APPLICATION_ID_AQUI",
  "details": "Descripción del estado",
  "state": "Estado adicional o null",
  "large_image": "nombre_imagen",
  "large_text": "Texto que aparece al pasar el mouse",
  "manual_active": null,
  "auto_detect_file": true,
  "category": "Categoría del programa",
  "windowTitles": ["Título1", "Título2"],
  "description": "Descripción del programa"
}
```

## Cómo usar

Los usuarios de Neco Discord Presence pueden:

1. **Descargar programas**: Ver la lista de programas disponibles y descargarlos directamente desde la aplicación
2. **Compartir programas**: Subir sus propias configuraciones para que otros usuarios las puedan usar

## Nota importante

⚠️ **Application ID**: Cada usuario debe cambiar el `applicationId` por su propio Application ID de Discord Developer Portal.

⚠️ **Imágenes**: Las imágenes deben subirse manualmente al Discord Developer Portal del usuario.

## Contribuir

Los usuarios pueden compartir sus configuraciones directamente desde la aplicación Neco Discord Presence, o hacer un Pull Request manualmente.

### Cómo compartir desde la aplicación

1. Abre Neco Discord Presence
2. Selecciona un programa de tu lista
3. Haz clic en el botón "Compartir" en el panel derecho
4. Ingresa tu nombre o alias
5. La configuración se subirá automáticamente a la biblioteca

### Cómo contribuir manualmente

1. Crea un archivo JSON en la carpeta `programs/` con el formato mostrado arriba
2. Si tienes una imagen, súbela a la carpeta `images/`
3. Actualiza `programs.json` agregando la información del nuevo programa
4. Haz un Pull Request

## Notas importantes

- ⚠️ **Application ID**: Cada usuario debe cambiar el `applicationId` por su propio Application ID de Discord Developer Portal
- ⚠️ **Imágenes**: Las imágenes deben subirse manualmente al Discord Developer Portal del usuario
- ⚠️ **Formato**: Asegúrate de seguir el formato JSON correcto para que la aplicación pueda leer las configuraciones

## Licencia

Este repositorio es de código abierto y las configuraciones compartidas son de uso libre. Ver [LICENSE](LICENSE) para más detalles.

