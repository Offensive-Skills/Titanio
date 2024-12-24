### **Básico/Utilidades de Red/telnet.md**

# telnet

## Descripción

`telnet` es una herramienta de red utilizada para establecer conexiones TCP a través de la red. Aunque ha sido en gran medida reemplazada por protocolos más seguros como SSH, `telnet` todavía se utiliza para probar y depurar servicios de red, así como para acceder a sistemas antiguos que no soportan métodos de autenticación más modernos.

## Uso

```bash
telnet [opciones] host [puerto]
```

### Opciones principales

- `-l`: Especifica el nombre de usuario para la autenticación.
- `-a`: Usa autenticación automática.
- `-E`: No envía información de inicio de sesión al servidor.
- `-d`: Activa el modo de depuración.
- `-8`: Usa 8 bits de datos por byte.
- `-noopt`: Deshabilita opciones específicas del protocolo.

## Ejemplos

- Establecer una conexión Telnet a un servidor en el puerto 23:
  
  ```bash
  telnet ejemplo.com 23
  ```

- Conectarse a un servidor en el puerto 80 (HTTP) para probar una conexión web:
  
  ```bash
  telnet ejemplo.com 80
  ```

- Especificar un nombre de usuario al conectarse:
  
  ```bash
  telnet -l usuario ejemplo.com 23
  ```

- Activar el modo de depuración:
  
  ```bash
  telnet -d ejemplo.com 23
  ```

- Deshabilitar el envío de información de inicio de sesión:
  
  ```bash
  telnet -E ejemplo.com 23
  ```