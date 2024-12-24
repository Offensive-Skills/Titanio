### **Explotación de Active Directory/CrackMapExec.md**

# CrackMapExec

## Descripción

`CrackMapExec` (CME) es una herramienta de post-explotación para redes Windows. Permite automatizar la evaluación de la seguridad en redes empresariales, facilitando la enumeración de hosts, la explotación de vulnerabilidades y la ejecución de comandos remotos.

## Uso

```bash
cme [comandos] [opciones]
```

### Opciones principales

- `--target`: Especifica el objetivo (IP, rango o lista de hosts).
- `-u`, `--username`: Nombre de usuario para autenticación.
- `-p`, `--password`: Contraseña para autenticación.
- `--hashes`: Proporciona hashes NTLM para autenticación.
- `-d`, `--domain`: Define el dominio.
- `--exec-method`: Método de ejecución remota (e.g., smb, wmiexec).
- `-M`, `--module`: Especifica un módulo para ejecutar.
- `-h`, `--help`: Muestra la ayuda y opciones disponibles.

## Ejemplos

- Enumerar todos los usuarios en un dominio:
  
  ```bash
  cme smb 192.168.1.0/24 -u administrador -p Contraseña123 --users
  ```

- Ejecutar un comando remoto en múltiples hosts:
  
  ```bash
  cme smb 192.168.1.0/24 -u administrador -p Contraseña123 -x "ipconfig /all"
  ```

- Dump de hashes NTLM:
  
  ```bash
  cme smb 192.168.1.0/24 -u administrador -p Contraseña123 --hashes
  ```
