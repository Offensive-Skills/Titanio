### **Hacking Web/Escáneres de Vulnerabilidades Web/Nikto.md**

# Nikto

## Descripción

`Nikto` es un escáner de vulnerabilidades web de código abierto que realiza pruebas exhaustivas en servidores web para identificar problemas de seguridad conocidos, configuraciones incorrectas y archivos potencialmente peligrosos. Es una herramienta esencial para realizar evaluaciones de seguridad iniciales en aplicaciones web.

## Uso

```bash
nikto [opciones]
```

### Opciones principales

- `-h HOST`: Especifica el host objetivo para el escaneo.
- `-p PORT`: Define el puerto en el que se ejecuta el servidor web.
- `-ssl`: Realiza el escaneo sobre HTTPS.
- `-Tuning T`: Define el tipo de pruebas a realizar (e.g., 1 para archivos, 2 para plugins).
- `-output FILE`: Guarda los resultados del escaneo en un archivo especificado.
- `-Format FORMAT`: Define el formato del reporte (e.g., html, csv).
- `-v`: Modo verbose, muestra información detallada durante el escaneo.

## Ejemplos

- Escanear un host específico en el puerto 80:
  
  ```bash
  nikto -h http://example.com -p 80
  ```

- Escanear un host sobre HTTPS:
  
  ```bash
  nikto -h https://example.com -ssl
  ```

- Realizar pruebas específicas de archivos y plugins:
  
  ```bash
  nikto -h http://example.com -Tuning 1,2
  ```

- Guardar los resultados del escaneo en un archivo HTML:
  
  ```bash
  nikto -h http://example.com -output reporte_nikto.html -Format html
  ```

- Ejecutar el escaneo en modo verbose:
  
  ```bash
  nikto -h http://example.com -v
  ```
