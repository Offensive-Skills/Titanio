### **Básico/Compresión y Archivado/unzip.md**

# unzip

## Descripción

`unzip` es una herramienta utilizada para extraer archivos comprimidos en formato `.zip`. Permite descomprimir archivos individuales o todos los contenidos de un archivo zip de manera eficiente.

## Uso

```bash
unzip [opciones] archivo.zip
```

### Opciones principales

- `-d`: Especifica el directorio de destino para los archivos extraídos.
- `-l`: Lista el contenido del archivo zip sin extraer.
- `-v`: Modo detallado, muestra información adicional durante la extracción.
- `-o`: Sobrescribe los archivos existentes sin pedir confirmación.
- `-j`: Extrae los archivos sin recrear la estructura de directorios.
- `-n`: Nunca sobrescribe archivos existentes.

## Ejemplos

- Extraer todos los archivos en el directorio actual:
  
  ```bash
  unzip archivo.zip
  ```

- Extraer archivos en un directorio específico:
  
  ```bash
  unzip archivo.zip -d /ruta/destino/
  ```

- Listar el contenido del archivo zip:
  
  ```bash
  unzip -l archivo.zip
  ```

- Extraer archivos sobrescribiendo sin confirmación:
  
  ```bash
  unzip -o archivo.zip
  ```

- Extraer archivos sin recrear la estructura de directorios:
  
  ```bash
  unzip -j archivo.zip
  ```
