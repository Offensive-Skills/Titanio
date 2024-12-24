### **Básico/Gestión de Archivos/chown.md**

# chown

## Descripción

`chown` cambia el propietario y/o grupo de archivos y directorios.

## Uso

```bash
chown [opciones] propietario[:grupo] archivo
```

### Opciones principales

- `-R`: Aplica los cambios de forma recursiva a directorios.
- `-v`: Modo detallado, muestra las acciones realizadas.
- `--reference=archivo_referencia`: Aplica el propietario y grupo del archivo de referencia.

## Ejemplos

- Cambiar el propietario de un archivo:

  ```bash
  chown usuario archivo.txt
  ```

- Cambiar el propietario y el grupo de un archivo:

  ```bash
  chown usuario:grupo archivo.txt
  ```

- Cambiar propietario recursivamente en un directorio:

  ```bash
  chown -R usuario:grupo carpeta/
  ```

- Usar el grupo de un archivo de referencia:

  ```bash
  chown usuario: --reference=archivo_referencia.txt archivo.txt
  ```


