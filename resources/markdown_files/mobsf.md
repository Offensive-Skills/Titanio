### **Mobile_Security/Mobile_Security_Framework/Mobile_Security_Framework.md**

# Mobile Security Framework (MobSF)

## Descripción

`MobSF` es una herramienta automatizada de análisis estático y dinámico para aplicaciones móviles (Android, iOS, Windows). Facilita la detección de vulnerabilidades, análisis de seguridad y evaluación de aplicaciones móviles.

## Uso

```bash
./run.sh
```

### Opciones principales

- **Análisis Estático:**
  - Carga archivos APK, IPA o archivos de código fuente.
- **Análisis Dinámico:**
  - Requiere un dispositivo emulado o real para ejecutar la aplicación.
- **Informes:**
  - Genera informes detallados en formatos HTML, PDF y JSON.

## Ejemplos

- **Iniciar MobSF:**
  
  ```bash
  ./run.sh
  ```
  
- **Analizar un archivo APK:**
  
  1. Accede a la interfaz web en `http://localhost:8000`.
  2. Sube el archivo APK para análisis estático.

- **Realizar análisis dinámico:**
  
  1. Configura un dispositivo emulado en MobSF.
  2. Inicia la sesión de análisis dinámico desde la interfaz web.

