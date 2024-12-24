### **Cloud/ScoutSuite/scoutsuite.md**

# Scout Suite

## Descripción

`Scout Suite` es una herramienta de auditoría de seguridad de múltiples nubes que analiza configuraciones y despliegues en AWS, Azure, GCP y otros proveedores. Genera informes detallados sobre riesgos y vulnerabilidades.

## Uso

```bash
scout suite [opciones]
```

### Opciones principales

- `-A, --account nombre`: Especifica el nombre de la cuenta a auditar.
- `-b, --batch`: Ejecuta en modo no interactivo.
- `-o, --output directorio`: Define el directorio de salida para los informes.
- `-p, --provider proveedor`: Selecciona el proveedor de nube (aws, azure, gcp).

## Ejemplos

- **Auditar una cuenta de AWS y generar un informe en HTML:**

  ```bash
  scout suite --account mi_cuenta_aws --provider aws --output ./informes
  ```

- **Ejecutar Scout Suite en modo batch para Azure:**

  ```bash
  scout suite -A mi_cuenta_azure -p azure -b -o ./informes_azure
  ```
