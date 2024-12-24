### **Básico/Gestión de Archivos/mv.md**


## Descripción

`mv` mueve o renombra archivos y directorios.

## Uso

```bash
mv [opciones] origen destino
```

### Opciones principales

- `-i`: Solicita confirmación antes de sobrescribir.
- `-v`: Modo detallado, muestra las acciones realizadas.
- `-n`: No sobrescribe archivos existentes.

## Ejemplos

- Mover un archivo a otro directorio:

  ```bash
  mv archivo.txt /ruta/destino/
  ```

- Renombrar un archivo:

  ```bash
  mv archivo_viejo.txt archivo_nuevo.txt
  ```

- Mover con confirmación antes de sobrescribir:

  ```bash
  mv -i archivo.txt /ruta/destino/
  ```
