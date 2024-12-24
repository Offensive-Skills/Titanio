### **Herramientas de Seguridad/Enumeración/Seatbelt.md**

# Seatbelt

## Descripción

`Seatbelt` es una herramienta de recopilación de información y enumeración de seguridad para sistemas Windows. Está diseñada para operadores ofensivos que necesitan recopilar rápidamente información del sistema y posibles vulnerabilidades.

## Uso

Ejecutar el ejecutable con las opciones deseadas.

```cmd
Seatbelt.exe [opciones]
```

### Opciones principales

- `all`: Ejecuta todas las comprobaciones disponibles.
- `system`: Ejecuta comprobaciones relacionadas con el sistema.
- `user`: Ejecuta comprobaciones relacionadas con el usuario actual.
- `-group=grupo`: Especifica un grupo de comprobaciones (ej. `-group=cred`).
- `-output=file`: Especifica un archivo para guardar los resultados.

## Ejemplos

- Ejecutar todas las comprobaciones:

  ```cmd
  Seatbelt.exe all
  ```

- Ejecutar comprobaciones de credenciales:

  ```cmd
  Seatbelt.exe -group=cred
  ```

- Guardar resultados en un archivo:

  ```cmd
  Seatbelt.exe all -output=results.txt
  ```

