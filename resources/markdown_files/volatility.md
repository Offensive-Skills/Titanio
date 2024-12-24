### **Análisis Forense/Volatility/volatility.md**

# Volatility

## Descripción

**Volatility** es un framework avanzado de análisis de memoria RAM para sistemas Windows, Linux y macOS. Permite extraer información forense de volcados de memoria, como procesos activos, conexiones de red, módulos cargados y más.

## Uso

```bash
volatility -f volcado.mem --profile=perfil comando [opciones]
```

### Opciones principales

- `-f`: Especifica el archivo de volcado de memoria.
- `--profile`: Define el perfil del sistema operativo (ej. Win7SP1x64).
- `-h`: Muestra la ayuda y lista de comandos disponibles.
- `--plugins`: Especifica directorio de plugins personalizados.

### Comandos principales

- `pslist`: Lista los procesos activos.
- `pstree`: Muestra los procesos en forma de árbol.
- `netscan`: Enumera conexiones de red.
- `dlllist`: Lista las DLL cargadas por cada proceso.
- `filescan`: Busca objetos de tipo archivo en memoria.
- `hivelist`: Encuentra las ubicaciones de los registros en memoria.

## Ejemplos

- Listar procesos en un volcado de memoria:

  ```bash
  volatility -f memoria.raw --profile=Win7SP1x64 pslist
  ```

- Enumerar conexiones de red:

  ```bash
  volatility -f memoria.raw --profile=Win7SP1x64 netscan
  ```

