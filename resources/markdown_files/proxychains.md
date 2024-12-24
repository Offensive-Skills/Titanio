### **Herramientas de Red/Proxychains/proxychains.md**

# Proxychains

## Descripción

`proxychains` es una herramienta que fuerza a cualquier aplicación a través de un proxy como TOR, Danted, etc. Permite encaminar el tráfico de red de aplicaciones a través de proxies para anonimizar conexiones o acceder a redes restringidas.

## Uso

```bash
proxychains [opciones] aplicación [argumentos]
```

### Opciones principales

- `-f archivo`: Especifica un archivo de configuración distinto al predeterminado.
- `-q`: Modo silencioso, minimiza la salida.
- `-d`: Modo detallado, muestra información de depuración.

## Ejemplos

- Ejecutar nmap a través de proxychains:

  ```bash
  proxychains nmap -sT ejemplo.com
  ```

- Usar proxychains con un navegador:

  ```bash
  proxychains firefox
  ```

- Especificar un archivo de configuración personalizado:

  ```bash
  proxychains -f myproxychains.conf telnet ejemplo.com 80
  ```
