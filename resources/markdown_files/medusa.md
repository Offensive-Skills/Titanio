### **Herramientas de Seguridad/Cracking de Contraseñas/medusa.md**

# medusa

## Descripción

`medusa` es una herramienta rápida y masivamente paralela para realizar pruebas de autenticación remota. Soporta múltiples protocolos y está diseñada para ser modular y flexible en pruebas de penetración.

## Uso

```bash
medusa [opciones] -h objetivo -u usuario -p contraseña -M servicio
```

### Opciones principales

- `-h objetivo`: Especifica el host objetivo.
- `-H archivo_objetivos`: Especifica un archivo con una lista de hosts.
- `-u usuario`: Especifica un único nombre de usuario.
- `-U archivo_usuarios`: Especifica un archivo con una lista de usuarios.
- `-p contraseña`: Especifica una única contraseña.
- `-P archivo_contraseñas`: Especifica un archivo con una lista de contraseñas.
- `-M servicio`: Especifica el módulo (servicio/protocolo) a utilizar.
- `-n puerto`: Especifica el puerto a utilizar.
- `-t tareas`: Número de tareas paralelas (por defecto 4).

## Ejemplos

- Ataque contra SSH con usuario y lista de contraseñas:

  ```bash
  medusa -h ejemplo.com -u root -P passwords.txt -M ssh
  ```

- Ataque contra FTP utilizando listas de usuarios y contraseñas:

  ```bash
  medusa -H hosts.txt -U usuarios.txt -P passwords.txt -M ftp
  ```

- Especificar puerto personalizado y aumentar tareas paralelas:

  ```bash
  medusa -h ejemplo.com -u admin -P passwords.txt -M ssh -n 2222 -t 10
  ```
