### **Análisis Forense/ddrescue/ddrescue.md**

# ddrescue

## Descripción

`ddrescue` es una herramienta de recuperación de datos que copia datos de un archivo o dispositivo de bloque a otro, intentando rescatar los datos en caso de errores de lectura. Es útil para recuperar información de discos dañados o con sectores defectuosos.

## Uso

```bash
ddrescue [opciones] archivo_entrada archivo_salida archivo_log
```

### Opciones principales

- `-f`: Fuerza la escritura directa en el dispositivo de salida.
- `-n`: No hace una segunda pasada para recuperar datos erróneos.
- `-r N`: Especifica el número de reintentos en áreas con errores.
- `-v`: Modo detallado, muestra información adicional.
- `-B`: Invierte el orden de lectura (de atrás hacia adelante).

## Ejemplos

- Copiar datos de un disco a una imagen, registrando el progreso:

  ```bash
  ddrescue /dev/sda imagen_rescate.img log_rescate.log
  ```

- Hacer múltiples intentos en áreas dañadas:

  ```bash
  ddrescue -d -f -r 3 /dev/sda imagen_rescate.img log_rescate.log
  ```
