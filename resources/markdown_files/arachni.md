### **Hacking Web/Escáneres de Vulnerabilidades Web/Arachni.md**

# Arachni

## Descripción

`Arachni` es un escáner de vulnerabilidades web de código abierto diseñado para identificar y reportar fallos de seguridad en aplicaciones web. Soporta una amplia gama de pruebas, incluyendo inyecciones SQL, Cross-Site Scripting (XSS), y otros tipos de vulnerabilidades, ofreciendo una interfaz gráfica y una línea de comandos para facilitar su uso.

## Uso

```bash
arachni [opciones]
```

### Opciones principales

- `--url URL`: Especifica la URL objetivo para el escaneo.
- `--output-format FORMAT`: Define el formato del reporte (e.g., html, json, xml).
- `--output-path PATH`: Especifica el directorio donde se guardará el reporte.
- `--scope-sitemap`: Usa el sitemap para definir el alcance del escaneo.
- `--plugins PLUGINS`: Habilita o deshabilita plugins específicos.
- `--proxy PROXY_URL`: Usa un proxy específico durante el escaneo.
- `--authentication AUTH_METHOD`: Configura métodos de autenticación (e.g., form, http).
- `--help`: Muestra ayuda sobre las opciones disponibles.

## Ejemplos

- Iniciar un escaneo básico en una URL y generar un reporte en HTML:
  
  ```bash
  arachni --url "http://example.com" --output-format html --output-path ./reportes
  ```

- Realizar un escaneo utilizando el sitemap:
  
  ```bash
  arachni --url "http://example.com" --scope-sitemap
  ```

- Generar un reporte en formato JSON:
  
  ```bash
  arachni --url "http://example.com" --output-format json --output-path ./reportes
  ```

- Usar un proxy específico durante el escaneo:
  
  ```bash
  arachni --url "http://example.com" --proxy "http://127.0.0.1:8080"
  ```

- Configurar autenticación por formulario:
  
  ```bash
  arachni --url "http://example.com/login" --authentication form --data "username=admin&password=admin"
  ```
