### **Análisis Forense/MEMDump/memdump.md**

# memdump

## Descripción

`memdump` es una herramienta que permite volcar el contenido de la memoria de un proceso o del sistema completo. Se utiliza para capturar información volátil para análisis forense.

## Uso

```bash
memdump [opciones]
```

### Opciones principales

- `-p PID`: Especifica el ID del proceso a volcar.
- `-a`: Volca toda la memoria física.
- `-o archivo`: Especifica el archivo de salida.
- `-v`: Modo detallado.

## Ejemplos

- Volcar la memoria de un proceso específico:

  ```bash
  memdump -p 1234 -o proceso.dmp
  ```

- Volcar toda la memoria física:

  ```bash
  memdump -a -o memoria_total.dmp
  ```

