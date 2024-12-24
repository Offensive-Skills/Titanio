### **Hacking Web/Cross-Site Scripting (XSS)/xss_payloads.md**

# XSS Payloads

## Descripción

`XSS Payloads` es una colección de payloads diseñados para explotar vulnerabilidades Cross-Site Scripting (XSS) en aplicaciones web. Estos payloads varían desde simples scripts de alerta hasta scripts avanzados que pueden robar cookies, redirigir a usuarios o ejecutar comandos en el navegador.

## Uso

```bash
xss_payloads [opciones]
```

### Opciones principales

- `-f FILE`: Especifica un archivo que contiene los payloads.
- `-u URL`: Define la URL objetivo para inyectar los payloads.
- `--scan`: Ejecuta un escaneo automático con los payloads.
- `--custom PAYLOAD`: Agrega un payload personalizado a la lista.
- `--output FILE`: Guarda los resultados de las pruebas en un archivo especificado.
- `--verbose`: Muestra información detallada durante la ejecución.

## Ejemplos

- Escanear una URL utilizando una lista de payloads predeterminada:
  
  ```bash
  xss_payloads -u "http://example.com/search.php?q=test" --scan
  ```

- Usar un archivo personalizado con payloads y guardar los resultados:
  
  ```bash
  xss_payloads -u "http://example.com/comment.php" -f payloads_personalizados.txt --output resultados_xss.txt
  ```

- Agregar un payload personalizado y realizar un escaneo:
  
  ```bash
  xss_payloads -u "http://example.com/profile.php" --custom "<img src=x onerror=alert('XSS')>" --scan
  ```

- Ejecutar el escaneo en modo verbose para obtener más detalles:
  
  ```bash
  xss_payloads -u "http://example.com/login.php" --scan --verbose
  ```
