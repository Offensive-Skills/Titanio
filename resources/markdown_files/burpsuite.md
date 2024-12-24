### **Hacking Web/Escáneres de Vulnerabilidades Web/Burp_Suite.md**

# Burp Suite

## Descripción

`Burp Suite` es una plataforma integrada para pruebas de seguridad de aplicaciones web. Ofrece una variedad de herramientas que trabajan juntas para soportar todo el ciclo de pruebas, desde el mapeo inicial y análisis de superficie de ataque hasta la búsqueda y explotación de vulnerabilidades de seguridad.

## Uso

```bash
burpsuite [opciones]
```

### Opciones principales

- `-D PROXY_PORT`: Define el puerto del proxy de Burp Suite.
- `-c CONFIG_FILE`: Especifica un archivo de configuración personalizado.
- `-n`: Inicia Burp Suite sin cargar proyectos previos.
- `-t THREADS`: Define el número de hilos para ejecutar.
- `--headless`: Ejecuta Burp Suite en modo sin cabeza (headless).
- `--version`: Muestra la versión de Burp Suite.
- `--help`: Muestra ayuda sobre las opciones disponibles.

## Ejemplos

- Iniciar Burp Suite en modo proxy en el puerto 8080:
  
  ```bash
  burpsuite -D 8080
  ```

- Iniciar Burp Suite con un archivo de configuración específico:
  
  ```bash
  burpsuite -c config_burp.yaml
  ```

- Iniciar Burp Suite sin cargar proyectos previos:
  
  ```bash
  burpsuite -n
  ```

- Ejecutar Burp Suite en modo sin cabeza:
  
  ```bash
  burpsuite --headless
  ```

- Mostrar la versión de Burp Suite:
  
  ```bash
  burpsuite --version
  ```
