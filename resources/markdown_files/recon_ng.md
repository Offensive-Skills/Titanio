### **Miscelánea/Recolección de Información/Recon-ng.md**

# Recon-ng

## Descripción

`Recon-ng` es un framework modular de reconocimiento y recolección de información para realizar inteligencia de fuentes abiertas (OSINT). Ofrece una interfaz similar a Metasploit y permite la automatización de tareas de recolección de datos, facilitando la enumeración de objetivos en pruebas de penetración.

## Uso

```bash
recon-ng
```

### Comandos principales

- `workspaces`: Gestiona espacios de trabajo para diferentes objetivos.
- `modules`: Lista, carga y ejecuta módulos disponibles.
- `add`: Agrega datos al entorno de trabajo (e.g., dominios, IPs).
- `show`: Muestra información sobre el entorno y módulos.
- `exit`: Salir de Recon-ng.

### Opciones principales de módulos

- `load`: Carga un módulo específico.
- `set`: Configura parámetros del módulo.
- `run`: Ejecuta el módulo cargado.
- `options`: Muestra las opciones configurables del módulo.
- `help`: Muestra ayuda sobre comandos y módulos.

## Ejemplos

- Iniciar Recon-ng y crear un nuevo espacio de trabajo:
  
  ```bash
  recon-ng
  workspaces create ejemplo
  ```

- Agregar un dominio objetivo:
  
  ```bash
  add domains ejemplo.com
  ```

- Cargar y ejecutar el módulo de búsqueda de correos electrónicos:
  
  ```bash
  modules load recon/domains-contacts/google_search
  set SOURCE ejemplo.com
  run
  ```

- Exportar los resultados a un archivo CSV:
  
  ```bash
  modules load reporting/csv
  set FILENAME resultados.csv
  run
  ```

- Salir de Recon-ng:
  
  ```bash
  exit
  ```

