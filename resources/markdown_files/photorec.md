### **Análisis Forense/PhotoRec/photorec.md**

# PhotoRec

## Descripción

`PhotoRec` es una herramienta diseñada para recuperar archivos perdidos, incluyendo videos, documentos y archivos de discos duros, CD-ROM y fotos de tarjetas de memoria. Ignora el sistema de archivos y busca datos subyacentes, lo que permite recuperar archivos incluso si el sistema de archivos está dañado.

## Uso

```bash
photorec [dispositivo]
```

### Características principales

- **Recuperación de archivos**: Soporta más de 480 extensiones de archivos.
- **Independiente del sistema de archivos**: Funciona incluso si el sistema de archivos está severamente dañado.
- **Interfaz interactiva**: Fácil de usar mediante menús en la terminal.

## Ejemplos

- Iniciar PhotoRec y seguir las instrucciones:

  ```bash
  photorec
  ```

- Especificar un dispositivo o imagen al iniciar:

  ```bash
  photorec imagen.dd
  ```
