### **Básico/Utilidades de Red/ifconfig.md**

# ifconfig

## Descripción

`ifconfig` (interface configuration) es una herramienta de red utilizada para configurar, controlar y consultar las interfaces de red en sistemas Unix y Linux. Permite asignar direcciones IP, activar o desactivar interfaces, y visualizar la configuración de red actual.

## Uso

```bash
ifconfig [interfaz] [opciones]
```

### Opciones principales

- `up`: Activa una interfaz de red.
- `down`: Desactiva una interfaz de red.
- `inet`: Asigna una dirección IPv4 a una interfaz.
- `netmask`: Define la máscara de subred.
- `broadcast`: Define la dirección de broadcast.
- `mtu`: Establece el tamaño máximo de la unidad de transmisión.
- `promisc`: Activa el modo promiscuo en una interfaz.

## Ejemplos

- Mostrar la configuración de todas las interfaces de red:
  
  ```bash
  ifconfig
  ```

- Activar una interfaz de red:
  
  ```bash
  ifconfig eth0 up
  ```

- Desactivar una interfaz de red:
  
  ```bash
  ifconfig eth0 down
  ```

- Asignar una dirección IP a una interfaz:
  
  ```bash
  ifconfig eth0 inet 192.168.1.10 netmask 255.255.255.0
  ```

- Cambiar el tamaño máximo de la unidad de transmisión (MTU):
  
  ```bash
  ifconfig eth0 mtu 1400
  ```

- Activar el modo promiscuo en una interfaz:
  
  ```bash
  ifconfig eth0 promisc
  ```