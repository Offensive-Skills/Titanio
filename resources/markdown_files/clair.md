### **Container_Security/Clair/clair.md**

# Clair

## Descripción

`Clair` es un motor de análisis estático de vulnerabilidades para contenedores. Inspecciona imágenes Docker en busca de vulnerabilidades conocidas en paquetes y dependencias, integrándose con pipelines de CI/CD.

## Uso

```bash
clairctl [comando] [opciones]
```

### Comandos principales

- `clairctl analyze <imagen>`: Analiza una imagen Docker específica.
- `clairctl health`: Verifica el estado de Clair.
- `clairctl report <imagen>`: Genera un informe de vulnerabilidades para la imagen.

## Ejemplos

- **Analizar una imagen Docker:**

  ```bash
  clairctl analyze ubuntu:18.04
  ```

- **Verificar el estado de Clair:**

  ```bash
  clairctl health
  ```

- **Generar un informe de vulnerabilidades:**

  ```bash
  clairctl report nginx:latest
  ```
