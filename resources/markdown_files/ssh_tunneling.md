### **Herramientas de Red/SSH Tunneling/ssh_tunneling.md**

# SSH Tunneling

## Descripción

El **tunneling SSH** permite encapsular tráfico de red a través de una conexión SSH segura. Esto es útil para acceder a servicios protegidos, realizar port forwarding y crear conexiones seguras.

## Uso

```bash
ssh [opciones] usuario@servidor
```

### Opciones principales

- `-L [puerto_local]:destino:puerto_destino`: Port forwarding local.
- `-R [puerto_remoto]:destino:puerto_destino`: Port forwarding remoto.
- `-D [puerto]`: Crea un proxy SOCKS en el puerto especificado.
- `-N`: No ejecuta un comando remoto (útil para túneles).
- `-f`: Envía la sesión SSH al background.

## Ejemplos

- Port forwarding local:

  ```bash
  ssh -L 8080:localhost:80 usuario@servidor
  ```

  Accede al puerto 80 del servidor a través del puerto 8080 local.

- Port forwarding remoto:

  ```bash
  ssh -R 8080:localhost:80 usuario@servidor
  ```

  Permite que el servidor acceda al puerto 80 de tu máquina local a través de su puerto 8080.

- Crear un proxy SOCKS:

  ```bash
  ssh -D 1080 -N -f usuario@servidor
  ```
