### **Básico/Hacking Web/ffuf.md**

# ffuf (Fuzz Faster U Fool)

## Descripción

`ffuf` es una herramienta rápida y flexible para la exploración de directorios, archivos y parametrización de URLs mediante técnicas de fuzzing. Es especialmente útil para realizar pruebas de penetración y auditorías de seguridad en aplicaciones web, permitiendo descubrir recursos ocultos de manera eficiente.

## Uso

```bash
ffuf [opciones]
```

### Opciones principales

- `-u URL`: Define la URL objetivo con un marcador de posición (`FUZZ`).
- `-w WORDLIST`: Especifica la lista de palabras a utilizar para el fuzzing.
- `-t THREADS`: Establece el número de hilos concurrentes.
- `-e EXTENSIONS`: Añade extensiones de archivo para probar.
- `-mc CODES`: Filtra respuestas por códigos de estado HTTP.
- `-fc CODES`: Excluye respuestas con ciertos códigos de estado HTTP.
- `-o OUTPUT`: Define el archivo de salida para los resultados.
- `-of FORMATO`: Establece el formato del archivo de salida (json, html, etc.).

## Ejemplos

- Fuzzing de directorios:
  
  ```bash
  ffuf -u http://ejemplo.com/FUZZ -w /ruta/a/wordlist.txt
  ```

- Fuzzing con extensiones de archivo:
  
  ```bash
  ffuf -u http://ejemplo.com/FUZZ -w /ruta/a/wordlist.txt -e .php,.html,.txt
  ```

- Fuzzing y filtrar solo respuestas con código 200:
  
  ```bash
  ffuf -u http://ejemplo.com/FUZZ -w /ruta/a/wordlist.txt -mc 200
  ```

- Fuzzing y excluir respuestas con código 404:
  
  ```bash
  ffuf -u http://ejemplo.com/FUZZ -w /ruta/a/wordlist.txt -fc 404
  ```

- Guardar resultados en un archivo JSON:
  
  ```bash
  ffuf -u http://ejemplo.com/FUZZ -w /ruta/a/wordlist.txt -o resultados.json -of json
  ```
