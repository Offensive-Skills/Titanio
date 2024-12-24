### **Básico/Gestión de Archivos/mkdir.md**

# mkdir

## Descripción

`mkdir` crea nuevos directorios.

## Uso

```bash
mkdir [opciones] directorio
```

### Opciones principales

- `-p`: Crea directorios padres según sea necesario.
- `-v`: Modo detallado, muestra las acciones realizadas.

## Ejemplos

- Crear un solo directorio:

  ```bash
  mkdir nueva_carpeta
  ```

- Crear múltiples directorios a la vez:

  ```bash
  mkdir carpeta1 carpeta2 carpeta3
  ```

- Crear un directorio junto con sus padres:

  ```bash
  mkdir -p /ruta/padre/nueva_carpeta
  ```

- Crear un directorio en modo detallado:

  ```bash
  mkdir -v nueva_carpeta
  ```