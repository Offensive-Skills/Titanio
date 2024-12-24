### **Análisis Forense/TestDisk/testdisk.md**

# TestDisk

## Descripción

`TestDisk` es una herramienta de recuperación de datos que puede recuperar particiones perdidas y reparar sistemas de archivos. Es útil para recuperar discos que ya no son accesibles debido a errores en el software, ciertos tipos de virus o errores humanos.

## Uso

Ejecutar TestDisk desde la línea de comandos o utilizar su interfaz interactiva.

```bash
testdisk [logfile]
```

### Características principales

- **Recuperación de particiones**: Detecta y reconstruye tablas de particiones dañadas.
- **Reparación de sistemas de archivos**: Corrige errores en sistemas FAT32, NTFS, ext2/3/4, etc.
- **Recuperación de boot sectors**: Restaura sectores de arranque dañados.

## Ejemplos

- Iniciar TestDisk y seguir las opciones interactivas:

  ```bash
  testdisk
  ```

- Especificar un archivo de log:

  ```bash
  testdisk testdisk.log
  ```
