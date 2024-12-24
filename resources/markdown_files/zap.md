### **Hacking Web/Escáneres de Vulnerabilidades Web/OWASP_ZAP.md**

# OWASP ZAP

## Descripción

`OWASP ZAP` (Zed Attack Proxy) es una herramienta de código abierto diseñada para encontrar vulnerabilidades de seguridad en aplicaciones web. Es ideal tanto para principiantes como para profesionales de la seguridad, ofreciendo una interfaz amigable y capacidades avanzadas para realizar pruebas de penetración automatizadas y manuales.

## Uso

```bash
zap.sh [opciones]
```

### Opciones principales

- `-daemon`: Inicia ZAP en modo daemon, sin interfaz gráfica.
- `-port PORT`: Define el puerto en el que se ejecuta el proxy de ZAP.
- `-config KEY=VALUE`: Configura opciones específicas de ZAP.
- `-quickurl URL`: Ejecuta un escaneo rápido en la URL especificada.
- `-quickout FILE`: Guarda los resultados del escaneo rápido en un archivo.
- `--help`: Muestra ayuda sobre las opciones disponibles.

## Ejemplos

- Iniciar OWASP ZAP en modo daemon en el puerto 8080:
  
  ```bash
  zap.sh -daemon -port 8080
  ```

- Realizar un escaneo rápido en una URL y guardar los resultados en un archivo HTML:
  
  ```bash
  zap.sh -quickurl "http://example.com" -quickout reporte_zap.html
  ```

- Configurar una opción específica antes de iniciar ZAP:
  
  ```bash
  zap.sh -config api.key=mi_clave_api
  ```

- Mostrar la ayuda de OWASP ZAP:
  
  ```bash
  zap.sh --help
  ```

