### **Básico/Transferencia de Archivos/sftp.md**

# sftp

## Descripción

`sftp` (SSH File Transfer Protocol) es una herramienta de red utilizada para transferir archivos de forma segura entre el sistema local y un servidor remoto a través de una conexión SSH. Proporciona funcionalidades similares a FTP pero con cifrado para mayor seguridad.

## Uso

```bash
sftp [opciones] usuario@host
```

### Opciones principales

- `-b`: Ejecuta comandos desde un archivo batch.
- `-C`: Habilita la compresión de datos.
- `-P`: Especifica un puerto diferente al puerto SSH por defecto.
- `-i`: Usa una clave de identidad (archivo de clave privada) para la autenticación.
- `-o`: Define opciones adicionales de SSH.

## Ejemplos

- Conectarse a un servidor SFTP:
  
  ```bash
  sftp usuario@ejemplo.com
  ```

- Especificar un puerto diferente:
  
  ```bash
  sftp -P 2222 usuario@ejemplo.com
  ```

- Subir un archivo al servidor:
  
  ```bash
  sftp> put archivo.txt
  ```

- Descargar un archivo del servidor:
  
  ```bash
  sftp> get archivo.txt
  ```

- Listar archivos en el directorio remoto:
  
  ```bash
  sftp> ls
  ```

- Cambiar al directorio remoto:
  
  ```bash
  sftp> cd carpeta/
  ```

- Subir múltiples archivos:
  
  ```bash
  sftp> mput *.txt
  ```

- Descargar múltiples archivos:
  
  ```bash
  sftp> mget *.txt
  ```

- Salir del cliente SFTP:
  
  ```bash
  sftp> bye
  ```

- Ejecutar comandos desde un archivo batch:
  
  ```bash
  sftp -b comandos_sftp.txt usuario@ejemplo.com
  ```