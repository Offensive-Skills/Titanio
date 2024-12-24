### **Container_Security/DockerScan/dockerscan.md**

# DockerScan

## Descripción

`DockerScan` es una herramienta de escaneo de seguridad para imágenes Docker. Analiza vulnerabilidades, configuraciones inseguras y dependencias obsoletas en contenedores Docker.

## Uso

```bash
dockerscan [opciones] <imagen>
```

### Opciones principales

- `-f, --file Dockerfile`: Especifica un Dockerfile para análisis.
- `-o, --output archivo`: Guarda el informe en un archivo.
- `-q, --quiet`: Ejecuta en modo silencioso.
- `-v, --verbose`: Muestra detalles adicionales durante el escaneo.

## Ejemplos

- **Escanear una imagen Docker pública:**

  ```bash
  dockerscan nginx:latest
  ```

- **Analizar un Dockerfile y guardar el informe:**

  ```bash
  dockerscan -f Dockerfile -o informe_docker.txt
  ```

- **Ejecutar en modo detallado:**

  ```bash
  dockerscan -v mi_imagen:1.0
  ```

