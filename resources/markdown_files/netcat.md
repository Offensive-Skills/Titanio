### **Herramientas de Red/Netcat/netcat.md**

# Netcat

## Descripción

`netcat` es una herramienta versátil para lectura y escritura en conexiones de red utilizando protocolos TCP o UDP. Se utiliza para depuración de red, transferencia de archivos y creación de conexiones simples.

## Uso

```bash
nc [opciones] [host] [puerto]
```

### Opciones principales

- `-l`: Modo escucha, actúa como servidor.
- `-p`: Especifica el puerto local a utilizar.
- `-e`: Ejecuta un programa después de establecer conexión.
- `-u`: Utiliza el protocolo UDP en lugar de TCP.
- `-v`: Modo detallado, muestra información adicional.
- `-z`: Modo escaneo de puertos (sin enviar datos).

## Ejemplos

- Iniciar un listener en el puerto 1234:

  ```bash
  nc -l -p 1234
  ```

- Conectarse a un host en el puerto 1234:

  ```bash
  nc ejemplo.com 1234
  ```

- Transferir un archivo:

  **En el receptor:**

  ```bash
  nc -l -p 1234 > archivo_recibido.txt
  ```

  **En el remitente:**

  ```bash
  nc ejemplo.com 1234 < archivo_a_enviar.txt
  ```

- Escanear puertos abiertos:

  ```bash
  nc -z -v ejemplo.com 20-80
  ```
