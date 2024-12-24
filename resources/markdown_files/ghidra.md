### **Análisis de Malware/Ghidra.md**

# Ghidra

## Descripción

`Ghidra` es un framework de ingeniería inversa desarrollado por la Agencia de Seguridad Nacional de EE.UU. (NSA). Ofrece herramientas para el análisis de software, desensamblado, decompilación y depuración de binarios, soportando múltiples arquitecturas y formatos de archivo.

## Uso

```bash
ghidraRun
```

### Opciones principales

- **Interfaz gráfica**: Ghidra se utiliza principalmente a través de su interfaz gráfica de usuario.
- **Scripting**: Soporta scripts en Python y Java para automatizar tareas.
- **Extensiones**: Permite la adición de plugins para funcionalidades adicionales.

## Ejemplos

- Abrir un proyecto en Ghidra:

  1. Ejecuta `ghidraRun` para iniciar la interfaz.
  2. Crea un nuevo proyecto o abre uno existente.
  3. Importa el binario que deseas analizar.

- Ejecutar un script en Ghidra:

  ```bash
  # Dentro de Ghidra, navega a Script Manager y ejecuta el script deseado.
  ```
