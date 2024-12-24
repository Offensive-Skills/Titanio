### **Herramientas de Red/RPC Client/rpcclient.md**

# rpcclient

## Descripción

`rpcclient` es una herramienta que permite ejecutar llamadas RPC (Remote Procedure Call) en servidores Windows. Se utiliza para interactuar con servicios y obtener información del sistema remoto.

## Uso

```bash
rpcclient [host] [opciones]
```

### Opciones principales

- `-U`: Especifica el nombre de usuario.
- `-N`: No solicita contraseña.
- `-c`: Ejecuta comandos específicos al conectar.

## Ejemplos

- Conectarse a un servidor sin autenticación:

  ```bash
  rpcclient ejemplo.com -N
  ```

- Conectarse con un usuario y ejecutar un comando:

  ```bash
  rpcclient ejemplo.com -U usuario -c 'querydominfo'
  ```

- Enumerar usuarios:

  ```bash
  rpcclient ejemplo.com -U usuario -c 'enumdomusers'
  ```

