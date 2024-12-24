### **Hacking Web/Cross-Site Scripting (XSS)/BeEF.md**

# BeEF

## Descripción

`BeEF` (Browser Exploitation Framework) es una herramienta de explotación centrada en navegadores que permite a los atacantes controlar navegadores web a través de vulnerabilidades XSS. Facilita la ejecución de módulos de explotación y la manipulación de sesiones de usuario comprometidas.

## Uso

```bash
beef [opciones]
```

### Opciones principales

- `-x CONFIG`: Especifica el archivo de configuración.
- `-f`: Inicia en modo foreground.
- `-c PORT`: Define el puerto en el que se ejecuta el servidor BeEF.
- `-d`: Habilita el modo debug para obtener información detallada.
- `--no-browser`: No abre automáticamente el navegador al iniciar.
- `--help`: Muestra ayuda sobre las opciones disponibles.

## Ejemplos

- Iniciar BeEF con un archivo de configuración específico:
  
  ```bash
  beef -x config.yaml
  ```

- Iniciar BeEF en modo debug:
  
  ```bash
  beef -d
  ```

- Iniciar BeEF en un puerto personalizado (por ejemplo, 3000):
  
  ```bash
  beef -c 3000
  ```

- Iniciar BeEF sin abrir el navegador automáticamente:
  
  ```bash
  beef --no-browser
  ```
