### **Wireless/Inssider/inssider.md**

# Inssider

## Descripción

`Inssider` es una herramienta de análisis de redes Wi-Fi que proporciona información detallada sobre la intensidad de la señal, la estabilidad de la conexión y la calidad del canal. Es útil para optimizar la configuración de redes inalámbricas y detectar problemas de rendimiento.

## Uso

```bash
inssider [opciones]
```

### Opciones principales

- `-i interfaz`: Selecciona la interfaz de red inalámbrica a utilizar.
- `-c canal`: Define el canal para el análisis.
- `-d tiempo`: Establece la duración del análisis en segundos.
- `-o archivo_salida`: Guarda los resultados en un archivo.
- `--help`: Muestra la ayuda y las opciones disponibles.

## Ejemplos

- Analizar la calidad de la señal en la interfaz wlan0 durante 60 segundos:

  ```bash
  inssider -i wlan0 -d 60
  ```

- Escanear el canal 6 y guardar los resultados:

  ```bash
  inssider -c 6 -o resultados.txt
  ```

- Iniciar un análisis detallado en la interfaz wlan1:

  ```bash
  inssider -i wlan1 -d 120 -v
  ```
