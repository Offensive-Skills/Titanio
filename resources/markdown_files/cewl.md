### **Hacking Web/Fuerza Bruta y Enumeración/CeWL.md**

# CeWL

## Descripción

`CeWL` es una herramienta que genera listas de palabras personalizadas a partir de sitios web. Analiza el contenido de una página web para extraer palabras que pueden ser utilizadas en ataques de fuerza bruta, como en el cracking de contraseñas.

## Uso

```bash
cewl [opciones] URL
```

### Opciones principales

- `-w`: Define el archivo de salida para guardar la lista de palabras.
- `-d`: Establece la profundidad máxima de enlaces a seguir.
- `-m`: Especifica el tamaño mínimo de las palabras a extraer.
- `-c`: Indica que la lista debe estar en formato clásico (una palabra por línea).
- `-n`: Elimina las palabras duplicadas.
- `--no-recurse`: No sigue los enlaces, analiza solo la página proporcionada.
- `-t`: Define el número de hilos a utilizar.

## Ejemplos

- Generar una lista de palabras a partir de una URL y guardar en un archivo:

  ```bash
  cewl -w lista_palabras.txt http://example.com
  ```

- Generar una lista con una profundidad de 2 enlaces:

  ```bash
  cewl -d 2 -w lista_palabras.txt http://example.com
  ```

- Generar una lista con palabras de al menos 5 caracteres:

  ```bash
  cewl -m 5 -w lista_palabras.txt http://example.com
  ```

- Generar una lista sin duplicados y en formato clásico:

  ```bash
  cewl -n -c -w lista_palabras.txt http://example.com
  ```
