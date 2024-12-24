### **Básico/Transferencia de Archivos/ftp.md**

# ftp

## Descripción

`ftp` es una herramienta de línea de comandos utilizada para transferir archivos entre el sistema local y un servidor FTP (File Transfer Protocol). Permite subir, descargar, listar y gestionar archivos en el servidor de manera interactiva.

## Uso

```bash
ftp [opciones] host
```

### Opciones principales

- `-n`: No realiza el inicio de sesión automático.
- `-v`: Modo detallado, muestra la conversación con el servidor.
- `-i`: Desactiva las confirmaciones interactivas.
- `-p`: Usa modo pasivo para la transferencia.
- `-s:archivo`: Lee comandos de un archivo.
- `-g`: Desactiva la expansión de globs.

## Ejemplos

- Conectarse a un servidor FTP:
  
  ```bash
  ftp ejemplo.com
  ```

- Subir un archivo al servidor:
  
  ```bash
  ftp> put archivo.txt
  ```

- Descargar un archivo del servidor:
  
  ```bash
  ftp> get archivo.txt
  ```

- Listar archivos en el directorio remoto:
  
  ```bash
  ftp> ls
  ```

- Cambiar al directorio remoto:
  
  ```bash
  ftp> cd carpeta/
  ```

- Subir múltiples archivos:
  
  ```bash
  ftp> mput *.txt
  ```

- Descargar múltiples archivos:
  
  ```bash
  ftp> mget *.txt
  ```

- Salir del cliente FTP:
  
  ```bash
  ftp> bye
  ```

- Usar un archivo de comandos para automatizar la conexión:
  
  ```bash
  ftp -n ejemplo.com < comandos_ftp.txt
  ```