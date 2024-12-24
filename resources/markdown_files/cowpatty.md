### **Wireless/Cowpatty/cowpatty.md**

# Cowpatty

## Descripción

`Cowpatty` es una herramienta de código abierto utilizada para realizar ataques de diccionario en redes Wi-Fi protegidas con WPA/WPA2. Permite intentar descifrar la contraseña de una red mediante la utilización de listas de palabras predefinidas.

## Uso

```bash
cowpatty [opciones]
```

### Opciones principales

- `-r archivo.cap`: Especifica el archivo de captura que contiene el handshake de la red Wi-Fi.
- `-S`: Utiliza un ataque de diccionario predefinido.
- `-C ESSID`: Especifica el nombre de la red Wi-Fi (ESSID).
- `-f archivo_diccionario`: Define el archivo de diccionario a utilizar en el ataque.
- `-x`: Fuerza el uso de WPA en lugar de WPA2.
- `-q`: Modo silencioso, reduce la salida de información.

## Ejemplos

- Realizar un ataque de diccionario usando un archivo de captura y un diccionario específico:

  ```bash
  cowpatty -r captura.cap -C MiRedWiFi -f diccionario.txt
  ```

- Usar el ataque de diccionario predefinido:

  ```bash
  cowpatty -r captura.cap -C MiRedWiFi -S
  ```

- Forzar el uso de WPA en el ataque:

  ```bash
  cowpatty -r captura.cap -C MiRedWiFi -f diccionario.txt -x
  ```
