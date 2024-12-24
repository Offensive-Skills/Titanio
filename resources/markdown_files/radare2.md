### **Análisis de Malware/Radare2.md**

# Radare2

## Descripción

`Radare2` es un framework de ingeniería inversa de código abierto que proporciona herramientas para el análisis de binarios, depuración, desensamblado y manipulación de archivos ejecutables. Es altamente configurable y extensible, adecuado para análisis estático y dinámico.

## Uso

```bash
radare2 [opciones] archivo
```

### Opciones principales

- `-A`: Realiza un análisis completo al abrir el archivo.
- `-d`: Inicia en modo depuración.
- `-e`: Ejecuta comandos al iniciar.
- `-c`: Ejecuta comandos específicos.

## Ejemplos

- Abrir un archivo para análisis:

  ```bash
  radare2 -A ejemplo.exe
  ```

- Iniciar Radare2 en modo depuración:

  ```bash
  radare2 -d ejemplo.exe
  ```

- Realizar un análisis y listar funciones:

  ```bash
  radare2 -A ejemplo.exe -c "afl"
  ```

