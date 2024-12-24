### **Ataques de Pass-the-Hash/WMIExec.md**

# WMIExec

## Descripción

`WMIExec` es una herramienta que utiliza Windows Management Instrumentation (WMI) para ejecutar comandos de manera remota en sistemas Windows. Facilita la administración y ejecución de tareas sin necesidad de instalar agentes adicionales.

## Uso

```bash
wmiexec.py [opciones]
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
  wmiexec.py usuario:Contraseña123@192.168.1.10 -c "ipconfig /all"
  ```

- Ejecutar un comando remoto usando hashes NTLM:
  
  ```bash
  wmiexec.py usuario:HASH_NTLM@192.168.1.10 -c "net user"
  ```
