### **Mobile_Security/ApkTool/apktool.md**

# ApkTool

## Descripción

`ApkTool` es una herramienta de código abierto para descompilar y recompilar aplicaciones Android (APK). Permite analizar y modificar recursos, como archivos XML y gráficos, facilitando la ingeniería inversa y la personalización de aplicaciones.

## Uso

```bash
apktool [opciones] <comando> <archivo.apk>
```

### Opciones principales

- `d`: Descompilar un APK.
- `b`: Recompilar un APK.
- `-o`: Especifica el directorio de salida.
- `-f`: Fuerza la descompilación incluso si hay errores.

## Ejemplos

- **Descompilar un APK:**
  
  ```bash
  apktool d app.apk -o app_descompilada
  ```

- **Recompilar un APK:**
  
  ```bash
  apktool b app_descompilada -o app_recompilada.apk
  ```

- **Forzar la descompilación:**
  
  ```bash
  apktool d app.apk -f -o app_descompilada
  ```
