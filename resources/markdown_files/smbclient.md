### **Herramientas de Red/SMB Client/smbclient.md**

# smbclient

## Descripción

`smbclient` es una herramienta que permite interactuar con recursos compartidos SMB/CIFS en redes Windows. Actúa de manera similar a un cliente FTP para acceder a archivos y directorios compartidos.

## Uso

```bash
smbclient //[host]/[recurso] [opciones]
```

### Opciones principales

- `-U`: Especifica el nombre de usuario.
- `-L`: Lista los recursos compartidos en el host.
- `-N`: No solicita contraseña (útil para recursos públicos).
- `-W`: Especifica el dominio o grupo de trabajo.
- `-c`: Ejecuta comandos específicos.

## Ejemplos

- Listar recursos compartidos en un host:

  ```bash
  smbclient -L ejemplo.com -U usuario
  ```

- Conectarse a un recurso compartido:

  ```bash
  smbclient //ejemplo.com/compartido -U usuario
  ```

- Descargar un archivo desde el recurso compartido:

  ```bash
  smbclient //ejemplo.com/compartido -U usuario -c 'get archivo.txt'
  ```
