### **Container_Security/Anchore/anchore.md**

# Anchore

## Descripción

`Anchore` es una plataforma de seguridad para contenedores que realiza análisis detallados de imágenes Docker. Evalúa políticas de seguridad, detecta vulnerabilidades y asegura el cumplimiento de estándares antes del despliegue.

## Uso

```bash
anchore-cli [comando] [opciones]
```

### Comandos principales

- `anchore-cli image add <imagen>`: Añade una imagen para análisis.
- `anchore-cli image list`: Lista las imágenes analizadas.
- `anchore-cli evaluate check <imagen>`: Evalúa una imagen contra políticas definidas.
- `anchore-cli report get <imagen>`: Obtiene el informe de análisis de una imagen.

## Ejemplos

- **Añadir una imagen Docker para análisis:**

  ```bash
  anchore-cli image add alpine:3.12
  ```

- **Listar imágenes analizadas:**

  ```bash
  anchore-cli image list
  ```

- **Evaluar una imagen contra políticas de seguridad:**

  ```bash
  anchore-cli evaluate check alpine:3.12
  ```

- **Obtener un informe detallado:**

  ```bash
  anchore-cli report get alpine:3.12
  ```

