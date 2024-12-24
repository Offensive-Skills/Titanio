### **Mobile_Security/QARK/qark.md**

# QARK

## Descripción

`QARK` (Quick Android Review Kit) es una herramienta de análisis estático para aplicaciones Android que identifica vulnerabilidades de seguridad y malas prácticas en el código fuente y archivos APK.

## Uso

```bash
qark --apk app.apk --source app_source/
```

### Opciones principales

- `--apk`: Especifica el archivo APK a analizar.
- `--source`: Define el directorio del código fuente.
- `--report`: Guarda el informe de análisis en un archivo.
- `--no-extract`: Evita extraer el APK antes del análisis.

## Ejemplos

- **Analizar un APK y generar un informe:**
  
  ```bash
  qark --apk app.apk --report informe_qark.html
  ```

- **Analizar el código fuente de una aplicación:**
  
  ```bash
  qark --source app_source/ --report informe_qark.html
  ```

- **Ejecutar QARK sin extraer el APK:**
  
  ```bash
  qark --apk app.apk --no-extract --report informe_qark.html
  ```
