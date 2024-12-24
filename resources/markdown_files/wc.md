### **Básico/Procesamiento de Texto/wc.md**


# wc

## Descripción

`wc` cuenta líneas, palabras y caracteres en archivos o entrada estándar.

## Uso

```bash
wc [opciones] archivo
```

### Opciones principales

- `-l`: Cuenta solo las líneas.
- `-w`: Cuenta solo las palabras.
- `-c`: Cuenta solo los bytes.
- `-m`: Cuenta caracteres (útil para multibyte).
- `-L`: Muestra la longitud de la línea más larga.

## Ejemplos

- Contar líneas, palabras y caracteres de un archivo:

  ```bash
  wc archivo.txt
  ```

- Contar solo líneas:

  ```bash
  wc -l archivo.txt
  ```

- Contar palabras en múltiples archivos:

  ```bash
  wc -w archivo1.txt archivo2.txt
  ```

- Mostrar la longitud de la línea más larga:

  ```bash
  wc -L archivo.txt
  ```
