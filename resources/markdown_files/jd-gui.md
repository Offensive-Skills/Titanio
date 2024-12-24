### **Reverse_Engineering/JD-GUI/jd-gui.md**

# JD-GUI

## Descripción

`JD-GUI` es una herramienta gráfica de código abierto utilizada para descompilar archivos JAR, Java de archivo o APK a código fuente Java legible. Permite a los desarrolladores y analistas de seguridad explorar y entender el código interno de aplicaciones Java y Android sin necesidad de tener acceso al código fuente original.

## Uso

`JD-GUI` ofrece una interfaz gráfica de usuario intuitiva.

1. **Iniciar JD-GUI:**
   - Ejecuta el archivo `jd-gui.exe` en Windows o el ejecutable correspondiente en otros sistemas.

2. **Abrir un Archivo:**
   - Haz clic en "File" > "Open" y selecciona el archivo JAR, APK o clase que deseas descompilar.

3. **Explorar el Código Fuente:**
   - Navega por los paquetes y clases en el panel de la izquierda para ver el código fuente descompilado en el panel derecho.

4. **Guardar el Código Fuente:**
   - Para exportar todo el código fuente, selecciona "File" > "Save All Sources" y elige el directorio de destino.

## Características principales

- Descompilación rápida y precisa de archivos Java y APK.
- Navegación fácil a través de paquetes, clases y métodos.
- Exportación del código fuente descompilado para su análisis offline.
- Soporte para versiones recientes de Java.

## Ejemplos

- **Descompilar un archivo JAR:**
  - Abre `mi_aplicacion.jar` en JD-GUI para ver el código fuente de las clases incluidas.

- **Exportar el código fuente de una APK:**
  - Abre `app.apk` en JD-GUI y selecciona "Save All Sources" para obtener todo el código Java descompilado.

- **Navegar por una clase específica:**
  - En el panel de la izquierda, expande el paquete `com.example` y selecciona `MainActivity` para ver su código fuente.
