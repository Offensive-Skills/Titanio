### **Programming_Languages/Bash/bash.md**

# Bash

## Descripción

`Bash` (Bourne Again Shell) es un intérprete de comandos y lenguaje de scripting para sistemas Unix y Linux. Es ampliamente utilizado para automatizar tareas, gestionar sistemas y escribir scripts de administración.

## Uso

```bash
bash [opciones] script.sh
```

### Opciones principales

- `-c`: Ejecuta comandos proporcionados como cadena.
- `-x`: Muestra los comandos y sus argumentos a medida que se ejecutan.
- `-e`: Termina el script si un comando falla.
- `-n`: Lee el script sin ejecutarlo para verificar errores de sintaxis.

## Ejemplos

- **Ejecutar un script Bash:**
  
  ```bash
  bash script.sh
  ```

- **Ejecutar comandos directamente:**
  
  ```bash
  bash -c "echo 'Hello, Bash!'"
  ```

- **Depurar un script mostrando cada comando:**
  
  ```bash
  bash -x script.sh
  ```

- **Verificar la sintaxis de un script sin ejecutarlo:**
  
  ```bash
  bash -n script.sh
  ```
