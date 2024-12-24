### **Miscelánea/Análisis de Malware/Cuckoo_Sandbox.md**

# Cuckoo Sandbox

## Descripción

`Cuckoo Sandbox` es una plataforma de análisis de malware de código abierto que permite ejecutar y analizar archivos sospechosos en un entorno aislado. Proporciona informes detallados sobre el comportamiento del malware, incluyendo cambios en el sistema, comunicaciones de red y actividades de archivos.

## Uso

```bash
cuckoo [comandos] [opciones]
```

### Comandos principales

- `cuckoo start`: Inicia la sandbox para análisis.
- `cuckoo submit`: Envía un archivo para análisis.
- `cuckoo status`: Verifica el estado de la sandbox.
- `cuckoo report`: Genera un informe del análisis.
- `cuckoo clean`: Limpia el entorno después del análisis.
- `cuckoo help`: Muestra la ayuda y opciones disponibles.

### Opciones principales

- `--config`: Archivo de configuración a utilizar.
- `--timeout`: Define el tiempo máximo de ejecución del análisis.
- `--package`: Selecciona el paquete de análisis específico.
- `--machine`: Define la máquina virtual a utilizar para el análisis.

## Ejemplos

- Iniciar la sandbox:
  
  ```bash
  cuckoo start
  ```

- Enviar un archivo para análisis:
  
  ```bash
  cuckoo submit malware.exe
  ```

- Verificar el estado de los análisis en curso:
  
  ```bash
  cuckoo status
  ```

- Generar un informe del análisis de un archivo específico:
  
  ```bash
  cuckoo report <ID_ANALISIS> --format json -o informe.json
  ```

- Limpiar el entorno después de los análisis:
  
  ```bash
  cuckoo clean
  ```
