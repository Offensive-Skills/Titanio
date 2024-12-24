### **Debugging/GDB/gdb.md**

# GDB

## Descripción

`GDB` (GNU Debugger) es un depurador de código abierto para programas escritos en C, C++ y otros lenguajes. Permite a los desarrolladores ejecutar programas paso a paso, inspeccionar variables, establecer puntos de interrupción y analizar el comportamiento de los programas para identificar y corregir errores.

## Uso

```bash
gdb [opciones] archivo_binario
```

### Opciones principales

- `-tui`: Inicia GDB con una interfaz de usuario de texto enriquecido.
- `-ex "comando"`: Ejecuta un comando GDB al iniciar.
- `-p pid`: Adjunta GDB a un proceso en ejecución mediante su PID.
- `-batch`: Ejecuta comandos en modo no interactivo.

## Comandos básicos

- `run [argumentos]`: Inicia la ejecución del programa.
- `break [función|línea]`: Establece un punto de interrupción.
- `continue`: Reanuda la ejecución hasta el siguiente punto de interrupción.
- `step`: Ejecuta la siguiente instrucción, entrando en funciones.
- `next`: Ejecuta la siguiente instrucción sin entrar en funciones.
- `print variable`: Muestra el valor de una variable.
- `backtrace`: Muestra la pila de llamadas actual.

## Ejemplos

- **Iniciar GDB con un binario:**
  ```bash
  gdb ./mi_programa
  ```

- **Establecer un punto de interrupción en la función `main`:**
  ```
  (gdb) break main
  ```

- **Iniciar la ejecución del programa:**
  ```
  (gdb) run
  ```

- **Avanzar una línea en el código:**
  ```
  (gdb) step
  ```

- **Imprimir el valor de una variable `x`:**
  ```
  (gdb) print x
  ```

- **Adjuntar GDB a un proceso con PID 1234:**
  ```bash
  gdb -p 1234
  ```

- **Ejecutar GDB en modo batch con comandos predefinidos:**
  ```bash
  gdb -batch -ex "break main" -ex "run" ./mi_programa
  ```
