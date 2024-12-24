### **Hacking Web/Fuerza Bruta y Enumeración/Gobuster.md**

# Gobuster

## Descripción

`gobuster` es una herramienta de fuerza bruta utilizada para descubrir directorios y archivos ocultos en servidores web, así como para enumerar subdominios. Es rápido y eficiente, soportando múltiples protocolos como HTTP, HTTPS, DNS y más.

## Uso

```bash
gobuster [modo] [opciones]
```

### Opciones principales

- `-u`: Especifica la URL objetivo.
- `-w`: Define el archivo de diccionario a utilizar.
- `-t`: Número de hilos a usar para la fuerza bruta.
- `-x`: Extensiones de archivo para añadir durante la búsqueda.
- `-s`: Especifica los códigos de estado HTTP a considerar como éxitos.
- `-o`: Define el archivo de salida para guardar los resultados.
- `-k`: Ignora los errores de certificado SSL.
- `-e`: Muestra el número exacto de caracteres en las respuestas.
- `--help`: Muestra la ayuda del comando.

## Ejemplos

- Enumerar directorios ocultos en una URL:

  ```bash
  gobuster dir -u http://example.com -w /ruta/diccionario.txt
  ```

- Enumerar subdominios usando DNS:

  ```bash
  gobuster dns -d example.com -w /ruta/diccionario_subdominios.txt -t 50
  ```

- Enumerar directorios con extensiones específicas:

  ```bash
  gobuster dir -u http://example.com -w /ruta/diccionario.txt -x php,html,txt
  ```

- Guardar los resultados en un archivo:

  ```bash
  gobuster dir -u http://example.com -w /ruta/diccionario.txt -o resultados.txt
  ```
