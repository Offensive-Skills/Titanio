### **Básico/Transferencia de Archivos/curl.md**

# curl

## Descripción

`curl` es una herramienta de línea de comandos utilizada para transferir datos desde o hacia un servidor utilizando diversos protocolos como HTTP, HTTPS, FTP, SFTP y más. Es altamente versátil y se utiliza para realizar solicitudes web, descargar archivos, subir datos y probar APIs.

## Uso

```bash
curl [opciones] URL
```

### Opciones principales

- `-O`: Guarda el archivo con el mismo nombre que en la URL.
- `-o`: Guarda el archivo con un nombre especificado.
- `-L`: Sigue redirecciones.
- `-C -`: Reanuda una descarga interrumpida.
- `-u`: Proporciona credenciales de usuario para autenticación.
- `-d`: Envía datos en una solicitud POST.
- `-X`: Especifica el método HTTP (e.g., GET, POST, PUT, DELETE).
- `-I`: Muestra solo los encabezados de la respuesta.
- `-H`: Añade un encabezado personalizado a la solicitud.
- `-k`: Ignora certificados SSL inválidos.

## Ejemplos

- Descargar un archivo y guardarlo con el mismo nombre:
  
  ```bash
  curl -O https://ejemplo.com/archivo.zip
  ```

- Descargar un archivo y guardarlo con un nombre específico:
  
  ```bash
  curl -o nuevo_nombre.zip https://ejemplo.com/archivo.zip
  ```

- Reanudar una descarga interrumpida:
  
  ```bash
  curl -C - -O https://ejemplo.com/archivo.zip
  ```

- Descargar una URL siguiendo redirecciones:
  
  ```bash
  curl -L -O https://ejemplo.com/archivo.zip
  ```

- Realizar una solicitud POST con datos:
  
  ```bash
  curl -X POST -d "usuario=ejemplo&contraseña=1234" https://ejemplo.com/login
  ```

- Enviar una solicitud GET con un encabezado personalizado:
  
  ```bash
  curl -H "Authorization: Bearer token123" https://ejemplo.com/api/data
  ```

- Mostrar solo los encabezados de la respuesta:
  
  ```bash
  curl -I https://ejemplo.com/
  ```

- Descargar un archivo ignorando certificados SSL inválidos:
  
  ```bash
  curl -k -O https://ejemplo.com/archivo.zip
  ```