### **Network_Security/Bettercap/bettercap.md**

# Bettercap

## Descripción

`Bettercap` es una herramienta de seguridad de red avanzada que reemplaza a herramientas como Ettercap. Permite realizar ataques de hombre en el medio (MITM), escaneo de red, sniffing de paquetes, spoofing y muchas otras funciones de análisis y manipulación de tráfico de red. Es altamente configurable y extensible mediante scripts.

## Uso

```bash
sudo bettercap [opciones]
```

### Opciones principales

- `-I interfaz`: Define la interfaz de red a utilizar.
- `-T objetivo`: Especifica la dirección IP del objetivo.
- `-X`: Activa el modo de escaneo pasivo de DNS.
- `-L`: Guarda los resultados del escaneo en un archivo.
- `--proxy`: Inicia un proxy HTTP/HTTPS para interceptar tráfico.
- `--help`: Muestra la ayuda y las opciones disponibles.

## Comandos en la interfaz interactiva

- `net.probe on`: Inicia el escaneo de la red.
- `arp.spoof on`: Activa el envenenamiento ARP para MITM.
- `dns.spoof on`: Activa el spoofing de DNS.
- `http.proxy on`: Inicia el proxy HTTP.
- `sessions.list`: Lista todas las sesiones activas.

## Ejemplos

- **Iniciar Bettercap con la interfaz wlan0:**
  ```bash
  sudo bettercap -I wlan0
  ```

- **Realizar un ataque ARP MITM a una IP específica:**
  ```
  bettercap > set arp.spoof.targets 192.168.1.100
  bettercap > arp.spoof on
  ```

- **Activar el proxy HTTP/HTTPS:**
  ```
  bettercap > http.proxy on
  ```

- **Iniciar un escaneo pasivo de DNS:**
  ```bash
  sudo bettercap -I wlan0 -X
  ```

- **Guardar los resultados del escaneo en un archivo:**
  ```bash
  sudo bettercap -I wlan0 -L resultados.txt
  ```
