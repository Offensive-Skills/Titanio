### **Hacking Web/Escáneres de Vulnerabilidades Web/Acunetix.md**

# Acunetix

## Descripción

`Acunetix` es una solución comercial de escaneo de vulnerabilidades web que detecta automáticamente una amplia gama de fallos de seguridad, incluyendo inyecciones SQL, Cross-Site Scripting (XSS), y otras vulnerabilidades OWASP. Ofrece una interfaz intuitiva y reportes detallados para facilitar la remediación de problemas de seguridad.

## Uso

```bash
acunetix [opciones]
```

### Opciones principales

- `-u URL`: Especifica la URL objetivo para el escaneo.
- `-c CONFIG_FILE`: Define un archivo de configuración personalizado.
- `-t THREADS`: Establece el número de hilos para ejecutar el escaneo.
- `-o OUTPUT_FILE`: Guarda los resultados del escaneo en un archivo especificado.
- `--login USER:PASSWORD`: Proporciona credenciales para acceder a áreas protegidas.
- `--fullscan`: Ejecuta un escaneo completo de todas las posibles vulnerabilidades.
- `--exclude PATH`: Excluye rutas específicas del escaneo.
- `--help`: Muestra ayuda sobre las opciones disponibles.

## Ejemplos

- Iniciar un escaneo completo en una URL específica:
  
  ```bash
  acunetix -u "http://example.com" --fullscan
  ```

- Guardar los resultados del escaneo en un archivo PDF:
  
  ```bash
  acunetix -u "http://example.com" -o reporte_acunetix.pdf
  ```

- Proporcionar credenciales para acceder a áreas protegidas:
  
  ```bash
  acunetix -u "http://example.com/admin" --login admin:password123
  ```

- Excluir rutas específicas del escaneo:
  
  ```bash
  acunetix -u "http://example.com" --exclude "/admin,/login"
  ```
