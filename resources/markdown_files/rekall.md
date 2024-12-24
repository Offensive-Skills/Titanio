### **Análisis Forense/Rekall/rekall.md**

# Rekall

## Descripción

**Rekall** es una herramienta de análisis de memoria RAM para sistemas Windows, Linux y macOS. Es un fork de Volatility que ofrece mejoras en rendimiento y características adicionales, facilitando el análisis forense de memoria.

## Uso

```bash
rekall [opciones] comando
```

### Opciones principales

- `-f`: Especifica el archivo de volcado de memoria.
- `--profile`: Define el perfil del sistema (se autodetecta en muchos casos).
- `--output`: Especifica el formato de salida (texto, JSON, HTML).

### Comandos principales

- `pslist`: Lista procesos activos.
- `pstree`: Muestra procesos en forma de árbol.
- `netstat`: Lista conexiones de red.
- `dlllist`: Muestra DLL cargadas por procesos.
- `filescan`: Escanea archivos en memoria.
- `dump`: Extrae información o memoria de procesos.

## Ejemplos

- Listar procesos:

  ```bash
  rekall -f memoria.raw pslist
  ```

- Mostrar conexiones de red:

  ```bash
  rekall -f memoria.raw netstat
  ```

