### **Herramientas de Red/Tunneling/chisel.md**

# chisel

## Descripción

`chisel` es una herramienta de tunneling que funciona mediante HTTP sobre WebSockets. Permite crear túneles TCP/UDP y port forwarding, facilitando el acceso a redes internas a través de conexiones salientes.

## Uso

```bash
# Servidor
chisel server [opciones]

# Cliente
chisel client [opciones] <servidor> <remoto:local>
```

### Opciones principales

- **Servidor**:
  - `--port`: Puerto en el que el servidor escucha.
  - `--reverse`: Permite túneles inversos desde el cliente.

- **Cliente**:
  - `--fingerprint`: Verificación del servidor.
  - `<servidor>`: Dirección del servidor en formato `host:puerto`.
  - `<remoto:local>`: Especifica el túnel a crear.

## Ejemplos

- Iniciar el servidor:

  ```bash
  chisel server --port 8000 --reverse
  ```

- Conectar un cliente y crear un túnel inverso:

  ```bash
  chisel client ejemplo.com:8000 R:8001:127.0.0.1:22
  ```

  Esto permite acceder al puerto 22 del cliente a través del puerto 8001 del servidor.


