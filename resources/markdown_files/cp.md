### **Básico/Gestión de Archivos/cp.md**

# cp

## Descripción

`cp` copia archivos y directorios de una ubicación a otra.

## Uso

```bash
cp [opciones] origen destino
```

### Opciones principales

- `-r` o `-R`: Copia directorios de forma recursiva.
- `-v`: Modo detallado, muestra el progreso de la copia.
- `-i`: Solicita confirmación antes de sobrescribir.
- `-u`: Copia solo cuando el archivo de origen es más nuevo que el de destino o cuando el archivo de destino no existe.
- `-p`: Preserva los atributos del archivo original.

## Ejemplos

- Copiar un archivo:

  ```bash
  cp archivo.txt /ruta/destino/
  ```

- Copiar un directorio de forma recursiva:

  ```bash
  cp -r carpeta /ruta/destino/
  ```

- Copiar con confirmación antes de sobrescribir:

  ```bash
  cp -i archivo.txt /ruta/destino/
  ```

- Copiar y preservar atributos:

  ```bash
  cp -p archivo.txt /ruta/destino/
  ```

