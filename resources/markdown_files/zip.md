### **Básico/Compresión y Archivado/zip.md**

# zip

## Descripción

`zip` es una herramienta de compresión que agrupa múltiples archivos y directorios en un archivo comprimido con extensión `.zip`. Es ampliamente utilizado para reducir el tamaño de los archivos y facilitar su distribución.

## Uso

```bash
zip [opciones] archivo.zip [archivos/directorios]
```

### Opciones principales

- `-r`: Comprime directorios de forma recursiva.
- `-v`: Modo detallado, muestra el progreso de las operaciones.
- `-e`: Encripta el archivo zip con una contraseña.
- `-9`: Usa la máxima compresión.
- `-u`: Actualiza archivos en el zip si han cambiado.
- `-m`: Mueve los archivos originales al zip, eliminándolos después.

## Ejemplos

- Comprimir un directorio:
  
  ```bash
  zip -r archivo.zip carpeta/
  ```

- Comprimir múltiples archivos:
  
  ```bash
  zip archivo.zip archivo1.txt archivo2.txt
  ```

- Comprimir con máxima compresión:
  
  ```bash
  zip -9 archivo.zip carpeta/
  ```

- Encriptar el archivo zip con una contraseña:
  
  ```bash
  zip -e archivo.zip archivo.txt
  ```

- Actualizar archivos en el zip:
  
  ```bash
  zip -u archivo.zip archivo_actualizado.txt
  ```