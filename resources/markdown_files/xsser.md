### **Hacking Web/Cross-Site Scripting (XSS)/XSSer.md**

# XSSer

## Descripción

`XSSer` es una herramienta automatizada para detectar y explotar vulnerabilidades de Cross-Site Scripting (XSS) en aplicaciones web. Ofrece múltiples técnicas de inyección y permite la personalización de payloads para identificar puntos débiles en la seguridad de las aplicaciones.

## Uso

```bash
xsser [opciones]
```

### Opciones principales

- `-u URL`: Especifica la URL objetivo para la prueba de XSS.
- `--auto`: Ejecuta pruebas automáticas sin intervención.
- `--payload PAYLOAD`: Define un payload personalizado para la inyección.
- `--cookie COOKIE`: Usa una cookie específica durante las pruebas.
- `--method METHOD`: Define el método de solicitud HTTP (GET o POST).
- `--data DATA`: Envía datos POST con la solicitud.
- `--crawl DEPTH`: Realiza crawling en la aplicación hasta la profundidad especificada.
- `--report REPORTFILE`: Guarda el reporte de vulnerabilidades detectadas.

## Ejemplos

- Escanear una URL en busca de vulnerabilidades XSS automáticamente:
  
  ```bash
  xsser --auto -u "http://example.com/page.php?id=1"
  ```

- Inyectar un payload personalizado y guardar el reporte:
  
  ```bash
  xsser -u "http://example.com/search.php?q=search" --payload "<script>alert('XSS')</script>" --report xss_report.txt
  ```

- Usar una cookie específica durante las pruebas:
  
  ```bash
  xsser -u "http://example.com/profile.php" --cookie "session=abcd1234"
  ```

- Realizar crawling hasta una profundidad de 3 niveles:
  
  ```bash
  xsser -u "http://example.com" --crawl 3
  ```

