### **Cloud/GCP_SDK/gcp_sdk.md**

# Google Cloud SDK

## Descripción

`Google Cloud SDK` es un conjunto de herramientas de línea de comandos para gestionar recursos y servicios de Google Cloud Platform (GCP). Incluye `gcloud`, `gsutil` y `bq` para interactuar con diferentes servicios de GCP.

## Uso

```bash
gcloud [comando] [subcomando] [opciones]
```

### Comandos principales

- `gcloud init`: Inicializa y configura el SDK.
- `gcloud compute instances list`: Lista las instancias de Compute Engine.
- `gcloud auth login`: Autentica al usuario en GCP.
- `gcloud projects create`: Crea un nuevo proyecto en GCP.

## Ejemplos

- **Inicializar el SDK de GCP:**

  ```bash
  gcloud init
  ```

- **Listar instancias de Compute Engine:**

  ```bash
  gcloud compute instances list
  ```

- **Autenticar en GCP:**

  ```bash
  gcloud auth login
  ```

- **Crear un nuevo proyecto:**

  ```bash
  gcloud projects create mi-proyecto
  ```
