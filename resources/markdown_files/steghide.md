### **Esteganografía/Herramientas de Ocultación de Datos/Steghide.md**

# Steghide

## Descripción

`Steghide` es una herramienta de esteganografía que permite ocultar datos dentro de archivos de medios como imágenes y audio. Soporta la encriptación de datos y ofrece opciones para comprimir y proteger la información oculta mediante contraseñas.

## Uso

```bash
steghide [comando] [opciones] archivo_portador
```

### Opciones principales

- `-e`: Cifra los datos antes de ocultarlos.
- `-d`: Extrae los datos ocultos de un archivo portador.
- `-sf`: Especifica el archivo portador.
- `-ef`: Define el archivo que se va a ocultar.
- `-cf`: Define el archivo de salida con los datos ocultos.
- `-p`: Define la contraseña para cifrar o descifrar los datos.
- `-z`: Establece el nivel de compresión.

## Ejemplos

- Ocultar un archivo dentro de una imagen con cifrado y contraseña:

  ```bash
  steghide embed -cf imagen.jpg -ef secreto.txt -p contraseña
  ```

- Extraer un archivo oculto de una imagen:

  ```bash
  steghide extract -sf imagen.jpg -p contraseña
  ```

- Ocultar un archivo sin cifrado:

  ```bash
  steghide embed -cf audio.mp3 -ef secreto.txt -p contraseña -e none
  ```
