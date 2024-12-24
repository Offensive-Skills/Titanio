### **Herramientas de Automatización/Sn1per.md**

# Sn1per

## Descripción

`Sn1per` es una herramienta de automatización de reconocimiento y escaneo para pruebas de penetración. Integra diversas utilidades de seguridad para realizar escaneos rápidos, enumeración de servicios, búsqueda de vulnerabilidades y recopilación de información detallada sobre el objetivo.

## Uso

```bash
sn1per [opciones] objetivo
```

### Opciones principales

- `-t`: Define el tipo de escaneo (e.g., full, fast).
- `-o`: Especifica el directorio de salida para los informes.
- `-m`: Modo de reconocimiento (e.g., web, dns).
- `--list-modules`: Lista todos los módulos disponibles.
- `--update`: Actualiza Sn1per a la última versión.

## Ejemplos

- Ejecutar un escaneo completo en un objetivo:

  ```bash
  sn1per -t full -o informes/ ejemplo.com
  ```

- Realizar un escaneo rápido:

  ```bash
  sn1per -t fast -o informes/ ejemplo.com
  ```

- Listar todos los módulos disponibles:

  ```bash
  sn1per --list-modules
  ```
