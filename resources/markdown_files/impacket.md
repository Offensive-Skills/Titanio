### **Explotación de Active Directory/Impacket.md**

# Impacket

## Descripción

`Impacket` es una colección de herramientas y bibliotecas de Python para interactuar con protocolos de red a bajo nivel. Es ampliamente utilizada para realizar pruebas de penetración y actividades de post-explotación en entornos Windows, facilitando la interacción con servicios como SMB, LDAP y Kerberos.

## Uso

```bash
impacket-command [opciones]
```

### Opciones principales

- `-h`, `--help`: Muestra la ayuda y las opciones disponibles.
- `-target`: Especifica el objetivo de la conexión.
- `-username`: Nombre de usuario para autenticación.
- `-password`: Contraseña para autenticación.
- `-hashes`: Proporciona hashes NTLM para autenticación.
- `-no-pass`: Omite la solicitud de contraseña.
- `-k`: Usa autenticación Kerberos.
- `-dc-ip`: Dirección IP del controlador de dominio.

## Ejemplos

- Enumerar los recursos compartidos en una máquina:
  
  ```bash
  smbclient.py usuario:password@ejemplo.com
  ```

- Ejecutar un comando remoto usando SMB:
  
  ```bash
  psexec.py usuario:password@ejemplo.com
  ```

- Obtener información del controlador de dominio:
  
  ```bash
  secretsdump.py usuario:password@ejemplo.com
  ```

