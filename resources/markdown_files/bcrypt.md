### **Seguridad/Cifrado/bcrypt.md**

# bcrypt

## Descripción

`bcrypt` es una herramienta de cifrado de archivos que utiliza el algoritmo de cifrado Blowfish para proteger datos sensibles. Está diseñada para ser simple y segura, proporcionando cifrado y descifrado desde la línea de comandos.

## Uso

```bash
bcrypt [opciones] archivo
```

### Opciones principales

- `-r`: Elimina el archivo original después del cifrado.
- `-c`: Cifra el archivo (opción por defecto).
- `-d`: Descifra el archivo.
- `-S`: Sobrescribe el archivo original con ceros antes de eliminarlo.

## Ejemplos

- Cifrar un archivo:

  ```bash
  bcrypt archivo.txt
  ```

- Descifrar un archivo:

  ```bash
  bcrypt -d archivo.txt.bfe
  ```

- Cifrar y eliminar el archivo original:

  ```bash
  bcrypt -r archivo.txt
  ```

**Nota**: `bcrypt` agrega la extensión `.bfe` a los archivos cifrados.
