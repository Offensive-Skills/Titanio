### **Hacking Web/Fuerza Bruta y Enumeración/Dirb.md**

# Dirb

## Descripción

`Dirb` es una herramienta de enumeración de directorios y archivos web que realiza solicitudes HTTP para descubrir recursos ocultos en servidores web. Es útil para identificar puntos de entrada no documentados, archivos de configuración sensibles y directorios de administración.

## Uso

```bash
dirb URL [wordlist] [opciones]
```

### Opciones principales

- `-o FILE`: Guarda los resultados del escaneo en un archivo especificado.
- `-w`: Usa una palabra clave para filtrar los resultados.
- `-r`: Rescanea recursos previamente encontrados.
- `-x EXTENSIONS`: Define extensiones de archivo adicionales a probar.
- `-z SIZING`: Define la estrategia de tamaño para las respuestas (e.g., linear, exponential).
- `-S`: Omite respuestas con ciertos códigos de estado HTTP.
- `-f`: Fuerza el escaneo incluso si el servidor no responde correctamente.
- `--threads N`: Define el número de hilos para acelerar el escaneo.

## Ejemplos

- Escanear una URL con la palabra lista predeterminada:
  
  ```bash
  dirb http://example.com
  ```

- Escanear una URL con una palabra lista personalizada y guardar los resultados:
  
  ```bash
  dirb http://example.com /path/to/wordlist.txt -o resultados_dirb.txt
  ```

- Probar extensiones de archivo adicionales como `.php`, `.bak` y `.txt`:
  
  ```bash
  dirb http://example.com /path/to/wordlist.txt -x .php,.bak,.txt
  ```

- Escanear con múltiples hilos para acelerar el proceso:
  
  ```bash
  dirb http://example.com /path/to/wordlist.txt --threads 10
  ```

- Filtrar respuestas con códigos de estado 403 y 404:
  
  ```bash
  dirb http://example.com /path/to/wordlist.txt -S 403,404
  ```
