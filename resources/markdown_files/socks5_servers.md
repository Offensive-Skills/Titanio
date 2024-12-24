### **Herramientas de Red/Servidores SOCKS5/socks5_servers.md**

# Servidores SOCKS5

## Descripción

Los **servidores SOCKS5** actúan como proxies que permiten enrutar tráfico de red a través de ellos. Son útiles para anonimizar conexiones y acceder a recursos en redes internas.

## Uso

Implementar un servidor SOCKS5 utilizando herramientas como `Dante`, `ss5` o mediante SSH.

### Opciones principales

- **Dante**:
  - Configuración en `/etc/danted.conf`.
  - Control de acceso mediante reglas.

- **SSH como servidor SOCKS5**:
  - Usar el parámetro `-D` para crear un proxy SOCKS.

## Ejemplos

- Iniciar un servidor SOCKS5 con SSH:

  ```bash
  ssh -D 1080 -N -f usuario@servidor
  ```

- Configurar Dante:

  - Editar `/etc/danted.conf` y definir interfaces y métodos de autenticación.
  - Iniciar el servicio:

    ```bash
    systemctl start danted
    ```
