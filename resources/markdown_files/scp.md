### **Básico/Transferencia de Archivos/scp.md**

# scp

## Descripción

`scp` (Secure Copy) es una herramienta de línea de comandos utilizada para copiar archivos y directorios de forma segura entre sistemas locales y remotos a través de una conexión SSH. Ofrece una transferencia rápida y segura de datos con cifrado.

## Uso

```bash
scp [opciones] origen destino
```

### Opciones principales

- `-r`: Copia directorios de forma recursiva.
- `-P`: Especifica un puerto diferente al puerto SSH por defecto.
- `-C`: Habilita la compresión de datos durante la transferencia.
- `-i`: Usa una clave de identidad (archivo de clave privada) para la autenticación.
- `-v`: Modo detallado, muestra información de depuración.
- `-q`: Modo silencioso, suprime mensajes de progreso.
- `-l`: Limita la tasa de transferencia en Kbit/s.

## Ejemplos

- Copiar un archivo desde el sistema local al servidor remoto:
  
  ```bash
  scp archivo.txt usuario@ejemplo.com:/ruta/destino/
  ```

- Copiar un archivo desde el servidor remoto al sistema local:
  
  ```bash
  scp usuario@ejemplo.com:/ruta/origen/archivo.txt /ruta/local/
  ```

- Copiar un directorio de forma recursiva al servidor remoto:
  
  ```bash
  scp -r carpeta/ usuario@ejemplo.com:/ruta/destino/
  ```

- Especificar un puerto diferente para la conexión SSH:
  
  ```bash
  scp -P 2222 archivo.txt usuario@ejemplo.com:/ruta/destino/
  ```

- Copiar un archivo usando una clave de identidad específica:
  
  ```bash
  scp -i ~/.ssh/id_rsa archivo.txt usuario@ejemplo.com:/ruta/destino/
  ```

- Limitar la tasa de transferencia a 500 Kbit/s:
  
  ```bash
  scp -l 500 archivo.txt usuario@ejemplo