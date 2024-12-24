### **Básico/Procesamiento de Texto/uniq.md**

# uniq

## Descripción

`uniq` elimina o reporta líneas repetidas en archivos ordenados.

## Uso

```bash
uniq [opciones] [archivo_entrada] [archivo_salida]
```

### Opciones principales

- `-c`: Cuenta las ocurrencias de cada línea.
- `-d`: Muestra solo las líneas duplicadas.
- `-u`: Muestra solo las líneas únicas.
- `-i`: Ignora mayúsculas y minúsculas al comparar.
- `-f N`: Omite los primeros N campos.
- `-s N`: Omite los primeros N caracteres de cada línea.

## Ejemplos

- Eliminar líneas duplicadas (el archivo debe estar ordenado):

  ```bash
  sort archivo.txt | uniq
  ```

- Contar las ocurrencias de cada línea:

  ```bash
  sort archivo.txt | uniq -c
  ```

- Mostrar solo líneas duplicadas:

  ```bash
  sort archivo.txt | uniq -d
  ```

- Mostrar solo líneas únicas:

  ```bash
  sort archivo.txt | uniq -u
  ```