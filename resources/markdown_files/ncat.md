### **Herramientas de Red/Ncat/ncat.md**

# Ncat

## Descripción

`ncat` es una herramienta de red que forma parte del paquete Nmap. Es similar a netcat pero con funcionalidades adicionales como soporte para SSL/TLS, proxying y más.

## Uso

```bash
ncat [opciones] [host] [puerto]
```

### Opciones principales

- `-l`: Modo escucha.
- `--listen`: Sinónimo de `-l`.
- `-e`: Ejecuta un programa al conectar.
- `--ssl`: Habilita cifrado SSL/TLS.
- `--proxy`: Especifica un proxy para conectar.
- `-k`: Mantiene el listener abierto para múltiples conexiones.
- `-u`: Utiliza UDP en lugar de TCP.
- `-v`: Modo detallado.

## Ejemplos

- Iniciar un listener con SSL:

  ```bash
  ncat --ssl -l 1234
  ```

- Conectarse a un listener SSL:

  ```bash
  ncat --ssl ejemplo.com 1234
  ```

- Crear un chat simple:

  **En el primer host:**

  ```bash
  ncat -l 1234
  ```

  **En el segundo host:**

  ```bash
  ncat ejemplo.com 1234
  ```

- Transferir un archivo:

  ```bash
  ncat --send-only ejemplo.com 1234 < archivo.txt
  ```
