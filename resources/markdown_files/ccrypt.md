### **Seguridad/Cifrado/ccrypt.md**

# ccrypt

## Descripción

`ccrypt` es una utilidad para cifrar y descifrar archivos y streams utilizando el algoritmo AES. Está diseñada para reemplazar herramientas antiguas como `crypt` y proporciona un cifrado seguro y moderno.

## Uso

```bash
ccrypt [opciones] archivo
```

### Opciones principales

- `-e`: Cifra el archivo (opción por defecto).
- `-d`: Descifra el archivo.
- `-c`: Trabaja con stdin/stdout (modo stream).
- `-k archivo`: Utiliza una frase de contraseña desde un archivo.
- `-r`: Procesa archivos en directorios recursivamente.
- `-x`: Solicita confirmación antes de sobrescribir archivos.

## Ejemplos

- Cifrar un archivo:

  ```bash
  ccrypt archivo.txt
  ```

- Descifrar un archivo:

  ```bash
  ccrypt -d archivo.txt.cpt
  ```

- Cifrar todos los archivos en un directorio:

  ```bash
  ccrypt -r *.txt
  ```

- Utilizar una frase de contraseña desde un archivo:

  ```bash
  ccrypt -k clave.txt archivo.txt
  ```

**Nota**: `ccrypt` agrega la extensión `.cpt` a los archivos cifrados.
