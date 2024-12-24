### **Análisis de Malware/IDA Pro.md**

# IDA Pro

## Descripción

`IDA Pro` (Interactive Disassembler) es una herramienta de desensamblado y depuración interactiva desarrollada por Hex-Rays. Es ampliamente utilizada en la ingeniería inversa para analizar binarios, entender el flujo de ejecución y detectar vulnerabilidades en el código.

## Uso

```bash
ida [opciones] archivo
```

### Opciones principales

- `-A`: Inicia el análisis automático del binario.
- `-B`: Genera un archivo binario de salida.
- `-S`: Ejecuta un script al iniciar.
- `-L`: Genera un log del análisis.

## Ejemplos

- Abrir un binario para análisis:

  ```bash
  ida ejemplo.exe
  ```

- Ejecutar IDA Pro con análisis automático y un script:

  ```bash
  ida -A -S=script.py ejemplo.exe
  ```

- Exportar el desensamblado a un archivo:

  ```bash
  ida -B ejemplo.exe
  ```
