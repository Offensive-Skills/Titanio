### **Cloud/CloudSploit/cloudsploit.md**

# CloudSploit

## Descripción

`CloudSploit` es una herramienta de escaneo de seguridad para entornos de nube que analiza configuraciones en AWS, Azure y GCP. Detecta vulnerabilidades y malas prácticas para mejorar la postura de seguridad.

## Uso

```bash
cloudsploit [comando] [opciones]
```

### Comandos principales

- `scan`: Realiza un escaneo de seguridad en la cuenta especificada.
- `report`: Genera un informe basado en el escaneo.
- `configure`: Configura las credenciales de acceso a la nube.

## Ejemplos

- **Escanear una cuenta de AWS:**

  ```bash
  cloudsploit scan aws
  ```

- **Generar un informe en formato JSON:**

  ```bash
  cloudsploit report --format json --output informe.json
  ```

- **Configurar credenciales para Azure:**

  ```bash
  cloudsploit configure azure --credentials azure_creds.json
  ```
