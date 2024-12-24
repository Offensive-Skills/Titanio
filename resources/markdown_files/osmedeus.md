### **Herramientas de Automatización/Osmedeus.md**

# Osmedeus

## Descripción

`Osmedeus` es una plataforma de automatización para pruebas de penetración que orquesta múltiples herramientas de seguridad. Facilita la recolección de información, escaneo de vulnerabilidades y explotación, proporcionando un flujo de trabajo integrado para evaluaciones de seguridad.

## Uso

```bash
osmedeus -t objetivo [opciones]
```

### Opciones principales

- `-t`: Define el objetivo para el escaneo.
- `-f`: Especifica el archivo de entrada con múltiples objetivos.
- `-d`: Define el nivel de detalle del escaneo.
- `--resume`: Reanuda un escaneo previamente interrumpido.
- `--update`: Actualiza Osmedeus y sus módulos.

## Ejemplos

- Ejecutar un escaneo básico en un objetivo:

  ```bash
  osmedeus -t ejemplo.com
  ```

- Realizar un escaneo con alto detalle:

  ```bash
  osmedeus -t ejemplo.com -d high
  ```

- Reanudar un escaneo interrumpido:

  ```bash
  osmedeus --resume
  ```
