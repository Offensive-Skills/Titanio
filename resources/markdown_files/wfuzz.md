### **Hacking Web/Fuerza Bruta y Enumeración/WFuzz.md**

# WFuzz

## Descripción

`WFuzz` es una herramienta de fuzzing y fuerza bruta diseñada para descubrir recursos web ocultos, como directorios, archivos, parámetros y más. Ofrece flexibilidad mediante la posibilidad de personalizar patrones de ataque y manejar respuestas HTTP complejas.

## Uso

```bash
wfuzz [opciones] [URL]
```

### Opciones principales

- `-c`: Muestra la salida coloreada.
- `-w`: Define el archivo de diccionario a utilizar.
- `-t`: Número de hilos a usar.
- `-u`: Especifica la URL objetivo, con marcadores de posición para los patrones.
- `-H`: Añade encabezados HTTP personalizados.
- `-d`: Envía datos POST en la solicitud.
- `--hw`: Filtra respuestas basadas en el tamaño del contenido (bytes).
- `--hl`: Filtra respuestas basadas en el número de líneas.
- `--mc`: Filtra respuestas basadas en códigos de estado HTTP.
- `--follow`: Sigue redirecciones HTTP.

## Ejemplos

- Enumerar directorios ocultos en una URL:

  ```bash
  wfuzz -c -w /ruta/diccionario.txt -u http://example.com/FUZZ/
  ```

- Enumerar archivos con extensiones específicas:

  ```bash
  wfuzz -c -w /ruta/diccionario.txt -u http://example.com/FUZZ.php
  ```

- Enumerar parámetros vulnerables a inyección SQL:

  ```bash
  wfuzz -c -w /ruta/diccionario_parametros.txt -d "username=admin&password=FUZZ" -u http://example.com/login
  ```

- Filtrar respuestas con códigos de estado 200:

  ```bash
  wfuzz -c -w /ruta/diccionario.txt -u http://example.com/FUZZ/ --mc 200
  ```
