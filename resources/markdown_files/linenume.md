### **Herramientas de Seguridad/Enumeración/LinEnum.md**

# LinEnum

## Descripción

`LinEnum` es un script de enumeración para sistemas Linux diseñado para verificar información del sistema y detectar posibles vías para escalada de privilegios. Ayuda a identificar configuraciones inseguras y vulnerabilidades en el sistema.

## Uso

Descargar el script y ejecutarlo en el sistema objetivo.

```bash
./LinEnum.sh [opciones]
```

### Opciones principales

- `-k`: Especifica categorías a ejecutar (ej. `-k sudo,passwd`).
- `-r`: Especifica un directorio para buscar permisos de escritura.
- `-e`: Ejecuta comprobaciones exhaustivas.
- `-s`: Salida mínima (silenciosa).
- `-t`: Salida detallada (verbose).

## Ejemplos

- Ejecutar con opciones por defecto:

  ```bash
  ./LinEnum.sh
  ```

- Ejecutar comprobaciones exhaustivas:

  ```bash
  ./LinEnum.sh -e
  ```

- Especificar categorías de comprobación:

  ```bash
  ./LinEnum.sh -k sudo,passwd
  ```

