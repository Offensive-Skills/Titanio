### **Desarrollo/FindBugs/findbugs.md**

# FindBugs

## Descripción

`FindBugs` es una herramienta de análisis estático para identificar defectos y vulnerabilidades en el código fuente de aplicaciones Java. Analiza bytecode y detecta posibles errores de programación que podrían conducir a fallos de seguridad, rendimiento o funcionalidad.

## Uso

FindBugs se puede utilizar a través de su interfaz gráfica, integración con IDEs como Eclipse, o desde la línea de comandos.

### Uso básico desde la línea de comandos

```bash
findbugs [opciones] archivo.jar
```

### Opciones principales

- `-textui`: Ejecuta FindBugs en modo texto.
- `-xml`: Genera un reporte en formato XML.
- `-html`: Genera un reporte en formato HTML.
- `-effort LEVEL`: Define el nivel de esfuerzo (min, default, max).
- `-threshold LEVEL`: Establece el umbral de reporte (Low, Medium, High).

## Ejemplos

- Ejecutar FindBugs en un archivo JAR y mostrar resultados en la terminal:
  
  ```bash
  findbugs -textui ejemplo.jar
  ```

- Generar un reporte HTML:
  
  ```bash
  findbugs -textui -html -output reporte.html ejemplo.jar
  ```

- Generar un reporte XML:
  
  ```bash
  findbugs -textui -xml -output reporte.xml ejemplo.jar
  ```

- Ejecutar con el nivel de esfuerzo máximo:
  
  ```bash
  findbugs -textui -effort max ejemplo.jar
  ```
