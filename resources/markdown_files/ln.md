### **Básico/Gestión de Archivos/ln.md**

# ln

## Descripción

`ln` crea enlaces entre archivos. Puede crear enlaces duros o simbólicos.

## Uso

```bash
ln [opciones] origen enlace
```

### Opciones principales

- `-s`: Crea un enlace simbólico.
- `-f`: Fuerza la creación, eliminando el enlace existente si es necesario.
- `-v`: Modo detallado, muestra las acciones realizadas.
- `-n`: No desreferencia enlaces simbólicos.

## Ejemplos

- Crear un enlace simbólico:

  ```bash
  ln -s /ruta/al/origen enlace_simbólico
  ```

- Crear un enlace duro:

  ```bash
  ln archivo.txt enlace_duro.txt
  ```

- Forzar la creación de un enlace simbólico, sobrescribiendo si existe:

  ```bash
  ln -sf /ruta/al/origen enlace_simbólico
  ```

- Crear un enlace simbólico en modo detallado:

  ```bash
  ln -sv /ruta/al/origen enlace_simbólico
  ```