### **Básico/Encriptación y Hashing/base64.md**

# base64

## Descripción

`base64` codifica o decodifica datos usando la representación Base64, común en transmisión de datos binarios.

## Uso

base64 [opciones] [archivo]

### Opciones principales

- `-d`, `--decode`: Decodifica datos Base64.
- `-w`: Especifica el ancho máximo de las líneas en la salida.
- `--ignore-garbage`: Ignora caracteres no válidos al decodificar.

## Ejemplos

- Codificar un archivo en Base64:

  base64 archivo.bin > archivo.b64

- Decodificar un archivo Base64:

  base64 -d archivo.b64 > archivo.bin

- Codificar una cadena de texto:

  echo "texto" | base64

- Decodificar una cadena Base64:

  echo "dGV4dG8K" | base64 -d

