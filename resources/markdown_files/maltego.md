### **Miscelánea/Recolección de Información/Maltego.md**

# Maltego

## Descripción

`Maltego` es una herramienta de análisis y minería de datos que facilita la visualización de relaciones y conexiones entre diferentes entidades en redes y sistemas. Es ampliamente utilizada para realizar recolección de información, análisis de redes y detección de amenazas en pruebas de penetración.

## Uso

```bash
maltego [opciones]
```

### Componentes principales

- **Transformaciones:** Scripts que permiten extraer datos de diferentes fuentes.
- **Entidades:** Objetos representativos como personas, dominios, IPs, etc.
- **Gráficos:** Visualizaciones que muestran las relaciones entre entidades.

### Opciones principales

- `-t`, `--transformation`: Ejecuta una transformación específica.
- `-e`, `--entity`: Define la entidad de inicio.
- `-g`, `--graph`: Genera un gráfico de las entidades y relaciones.
- `-o`, `--output`: Archivo de salida para resultados.
- `-h`, `--help`: Muestra la ayuda y opciones disponibles.

## Ejemplos

- Iniciar un nuevo proyecto y agregar una entidad de dominio:
  
  1. Abrir Maltego y crear un nuevo proyecto.
  2. Agregar una entidad de tipo "Domain" con el nombre `ejemplo.com`.
  3. Ejecutar transformaciones como "To DNS Names" o "To MX Records".

- Realizar una transformación de persona a correos electrónicos:
  
  1. Agregar una entidad de tipo "Person" con el nombre `Juan Pérez`.
  2. Ejecutar la transformación "To Email Addresses" para obtener correos asociados.

- Exportar el gráfico a un archivo PDF:
  
  ```bash
  maltego export --format pdf --output grafo.pdf
  ```

