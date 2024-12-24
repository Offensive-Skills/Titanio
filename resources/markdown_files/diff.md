### **Básico/Procesamiento de Texto/diff.md**

# diff

## Descripción

`diff` compara archivos línea por línea y muestra las diferencias.

## Uso

```bash
diff [opciones] archivo1 archivo2
```

### Opciones principales

- `-u`: Muestra el resultado en formato unificado.
- `-c`: Muestra el resultado en formato contextual.
- `-i`: Ignora diferencias en mayúsculas y minúsculas.
- `-w`: Ignora espacios en blanco.
- `--side-by-side`: Muestra las diferencias lado a lado.
- `-r`: Compara directorios de forma recursiva.

## Ejemplos

- Comparar dos archivos y mostrar diferencias:

  ```bash
  diff archivo1.txt archivo2.txt
  ```

- Mostrar diferencias en formato unificado:

  ```bash
  diff -u archivo1.txt archivo2.txt
  ```

- Comparar directorios de forma recursiva:

  ```bash
  diff -r directorio1/ directorio2/
  ```

- Ignorar diferencias en mayúsculas:

  ```bash
  diff -i archivo1.txt archivo2.txt
  ```
