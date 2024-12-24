### **Básico/Utilidades de Red/hostname.md**

# hostname

## Descripción

`hostname` es una herramienta de red utilizada para mostrar o establecer el nombre del host del sistema. El nombre del host es el identificador único de una máquina en una red, y es esencial para la comunicación y la administración de sistemas.

## Uso

```bash
hostname [opciones] [nuevo_nombre]
```

### Opciones principales

- `-f` o `--fqdn`: Muestra el nombre de dominio completamente calificado del host.
- `-i` o `--ip-address`: Muestra la dirección IP del host.
- `-I` o `--all-ip-addresses`: Muestra todas las direcciones IP del host.
- `-d` o `--domain`: Muestra el dominio del host.
- `-s` o `--short`: Muestra solo el nombre del host sin el dominio.
- `-F archivo`: Establece el nombre del host desde el contenido de un archivo.

## Ejemplos

- Mostrar el nombre actual del host:
  
  ```bash
  hostname
  ```

- Mostrar el nombre de dominio completamente calificado:
  
  ```bash
  hostname -f
  ```

- Mostrar la dirección IP del host:
  
  ```bash
  hostname -i
  ```

- Mostrar todas las direcciones IP del host:
  
  ```bash
  hostname -I
  ```

- Establecer un nuevo nombre de host:
  
  ```bash
  sudo hostname nuevo-host
  ```

- Establecer el nombre de host desde un archivo:
  
  ```bash
  sudo hostname -F /ruta/al/archivo
  ```