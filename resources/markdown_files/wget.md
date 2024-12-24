### **Básico/Transferencia de Archivos/wget.md**

# wget

## Descripción

`wget` es una herramienta de línea de comandos utilizada para descargar archivos desde la web. Soporta protocolos como HTTP, HTTPS y FTP, y es capaz de manejar descargas recursivas, reanudación de descargas interrumpidas y autenticación en sitios protegidos.

## Uso

```bash
wget [opciones] URL
```

### Opciones principales

- `-c`: Reanuda una descarga interrumpida.
- `-r`: Realiza descargas recursivas.
- `-P`: Especifica el directorio de destino para los archivos descargados.
- `-O`: Define el nombre del archivo de salida.
- `-b`: Ejecuta la descarga en segundo plano.
- `--limit-rate`: Limita la velocidad de descarga.
- `--user` y `--password`: Proporciona credenciales para la autenticación.
- `-np`: No sigue enlaces a directorios padres durante descargas recursivas.
- `-k`: Convierte enlaces para hacerlos navegables localmente.

## Ejemplos

- Descargar un archivo desde una URL:
  
  ```bash
  wget https://ejemplo.com/archivo.zip
  ```

- Reanudar una descarga interrumpida:
  
  ```bash
  wget -c https://ejemplo.com/archivo.zip
  ```

- Descargar recursivamente un sitio web:
  
  ```bash
  wget -r https://ejemplo.com/
  ```

- Descargar un archivo y guardarlo con un nombre específico:
  
  ```bash
  wget -O nuevo_nombre.zip https://ejemplo.com/archivo.zip
  ```

- Limitar la velocidad de descarga a 100KB/s:
  
  ```bash
  wget --limit-rate=100k https://ejemplo.com/archivo.zip
  ```

- Descargar un archivo en segundo plano:
  
  ```bash
  wget -b https://ejemplo.com/archivo.zip
  ```

- Descargar un archivo con autenticación:
  
  ```bash
  wget --user=usuario --password=contraseña https://ejemplo.com/archivo.zip
  ```