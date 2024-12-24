### **Hacking Web/Explotación de Sesiones/SSLstrip.md**

# SSLstrip

## Descripción

`SSLstrip` es una herramienta de tipo Man-in-the-Middle que degrada las conexiones HTTPS a HTTP, permitiendo la captura de información sensible que normalmente estaría cifrada. Es utilizada para realizar ataques de phishing y capturar credenciales de usuarios.

## Uso

```bash
sslstrip [opciones]
```

### Opciones principales

- `-l PORT`: Define el puerto donde SSLstrip escuchará las conexiones.
- `-w FILE`: Guarda los datos capturados en un archivo.
- `-f FILTER`: Aplica un filtro para capturar solo ciertos tipos de tráfico.
- `-v`: Modo detallado, muestra información adicional durante la ejecución.
- `--help`: Muestra ayuda y opciones disponibles.

## Ejemplos

- Iniciar SSLstrip en el puerto 8080 y guardar los datos capturados:

  ```bash
  sslstrip -l 8080 -w captura.log
  ```

- Iniciar SSLstrip con un filtro para capturar solo tráfico de login:

  ```bash
  sslstrip -l 8080 -f "login"
  ```

- Iniciar SSLstrip en modo detallado:

  ```bash
  sslstrip -l 8080 -v
  ```
