### **Hacking Web/Cross-Site Scripting (XSS)/xss_proxy.md**

# XSS-Proxy

## Descripción

`XSS-Proxy` es una herramienta que actúa como intermediario entre el navegador y el servidor web para interceptar y manipular tráfico, facilitando la detección y explotación de vulnerabilidades Cross-Site Scripting (XSS). Permite la inyección de payloads y la observación de respuestas en tiempo real.

## Uso

```bash
xss_proxy [opciones]
```

### Opciones principales

- `-l PORT`: Define el puerto en el que se ejecuta el proxy.
- `-t TARGET`: Especifica la URL objetivo que se va a interceptar.
- `--payload PAYLOAD`: Define un payload personalizado para la inyección.
- `--ssl`: Habilita el soporte para tráfico HTTPS.
- `--log FILE`: Guarda los registros de tráfico en un archivo especificado.
- `--help`: Muestra ayuda sobre las opciones disponibles.

## Ejemplos

- Iniciar XSS-Proxy en el puerto 8080 para interceptar tráfico a una URL específica:
  
  ```bash
  xss_proxy -l 8080 -t "http://example.com"
  ```

- Inyectar un payload personalizado en el tráfico interceptado:
  
  ```bash
  xss_proxy -l 8080 -t "http://example.com" --payload "<script>alert('XSS')</script>"
  ```

- Iniciar XSS-Proxy con soporte para HTTPS y guardar registros:
  
  ```bash
  xss_proxy -l 8443 -t "https://example.com" --ssl --log tráfico_xss.log
  ```
