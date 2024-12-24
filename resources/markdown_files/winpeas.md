### **Herramientas de Seguridad/Enumeración/winpeas.md**

# winPEAS

## Descripción

`winPEAS` es un script de enumeración en Windows que busca posibles vías para escalada de privilegios. Es útil para profesionales de seguridad que realizan pruebas en sistemas Windows para identificar configuraciones inseguras y vulnerabilidades.

## Uso

Ejecutar el script en el sistema objetivo.

```cmd
winpeas.exe [opciones]
```

### Opciones principales

- `cmd`: Ejecuta la versión de línea de comandos.
- `bat`: Ejecuta la versión en batch.
- `-h`: Muestra la ayuda y opciones disponibles.

## Ejemplos

- Ejecutar winPEAS estándar:

  ```cmd
  winpeas.exe
  ```

- Ejecutar versión de línea de comandos:

  ```cmd
  winpeas.exe cmd
  ```
