### **Ataques de Pass-the-Hash/PSEXEC.md**

# PsExec

## Descripción

`PsExec` es una herramienta de Microsoft que permite ejecutar procesos de manera remota en sistemas Windows. Es ampliamente utilizada para administración remota, pero también es una herramienta común en actividades de post-explotación debido a su capacidad para ejecutar comandos sin necesidad de instalar software adicional en el objetivo.

## Uso

```bash
psexec.py [opciones]
```

### Opciones principales

- `-target`: Dirección IP del objetivo.
- `-u`, `--username`: Nombre de usuario para autenticación.
- `-p`, `--password`: Contraseña para autenticación.
- `--hashes`: Proporciona hashes NTLM para autenticación.
- `-d`, `--domain`: Define el dominio.
- `-c`, `--command`: Comando a ejecutar remotamente.
- `-h`, `--help`: Muestra la ayuda y opciones disponibles.

## Ejemplos

- Ejecutar un comando remoto usando contraseña:
  
  ```bash
  psexec.py usuario:Contraseña123@192.168.1.10 -c "whoami"
  ```

- Transferir y ejecutar un archivo remoto:
  
  ```bash
  psexec.py usuario:Contraseña123@192.168.1.10 -c archivo.exe
  ```

- Ejecutar un comando remoto usando hashes NTLM:
  
  ```bash
  psexec.py usuario:HASH_NTLM@192.168.1.10 -c "netstat -an"
  ```
