### **Análisis Forense/Scalpel/scalpel.md**

# Scalpel

## Descripción

`scalpel` es una herramienta de recuperación de archivos basada en patrones, similar a foremost. Escanea medios digitales en busca de archivos eliminados o perdidos, utilizando encabezados y pies de página definidos en un archivo de configuración.

## Uso

```bash
scalpel [opciones] archivo_entrada -o directorio_salida
```

### Opciones principales

- `-c archivo_conf`: Especifica un archivo de configuración personalizado.
- `-o`: Define el directorio donde se guardarán los archivos recuperados.
- `-b`: Habilita el modo de fragmentos (para archivos fragmentados).
- `-v`: Modo detallado.

## Ejemplos

- Recuperar archivos usando la configuración por defecto:

  ```bash
  scalpel imagen.dd -o salida
  ```

- Especificar un archivo de configuración:

  ```bash
  scalpel -c scalpel.conf imagen.dd -o salida
  ```

