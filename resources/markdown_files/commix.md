### **Hacking Web/LFI y RCE/Commix.md**

# Commix

## Descripción

`Commix` (Command Injection Exploiter) es una herramienta automatizada para detectar y explotar vulnerabilidades de inyección de comandos en aplicaciones web. Permite la ejecución remota de comandos en servidores vulnerables, facilitando el acceso y control sobre sistemas comprometidos.

## Uso

```bash
commix [opciones]
```

### Opciones principales

- `-u URL`: Especifica la URL objetivo para la prueba de inyección de comandos.
- `--data=DATA`: Envía datos POST con la solicitud.
- `--level LEVEL`: Define el nivel de pruebas a ejecutar (1-5).
- `--risk RISK`: Define el nivel de riesgo de las pruebas (1-3).
- `--method METHOD`: Define el método de solicitud HTTP (GET o POST).
- `--batch`: Ejecuta en modo no interactivo, usando valores predeterminados.
- `--threads N`: Define el número de hilos para acelerar la explotación.
- `--timeout SECONDS`: Define el tiempo de espera para las solicitudes HTTP.

## Ejemplos

- Probar una URL para inyección de comandos:
  
  ```bash
  commix -u "http://example.com/page.php?cmd=ls"
  ```

- Usar datos POST en la solicitud y aumentar el nivel de pruebas:
  
  ```bash
  commix --data="username=admin&password=admin&cmd=ls" --level 3
  ```

- Ejecutar en modo no interactivo con un nivel de riesgo alto:
  
  ```bash
  commix -u "http://example.com/page.php?cmd=ping" --risk 3 --batch
  ```

- Usar múltiples hilos para acelerar la explotación:
  
  ```bash
  commix -u "http://example.com/page.php?cmd=whoami" --threads 10
  ```
