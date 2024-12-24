### **Análisis de Código/Matrix.md**

# Matrix

## Descripción

`Matrix` es una herramienta de análisis estático de código que ayuda a identificar vulnerabilidades, bugs y malas prácticas en el código fuente. Soporta múltiples lenguajes de programación y proporciona informes detallados para mejorar la calidad del software.

## Uso

```bash
matrix [opciones] archivo_o_directorio
```

### Opciones principales

- `-l`: Especifica el lenguaje de programación.
- `-o`: Define el archivo de salida para el informe.
- `-f`: Formato del informe (ej. JSON, HTML).
- `-v`: Modo detallado.

## Ejemplos

- Analizar todo el directorio actual para vulnerabilidades en Python:

  ```bash
  matrix -l python -o informe.json -f json .
  ```

- Generar un informe en HTML:

  ```bash
  matrix -l java -o informe.html -f html src/
  ```
