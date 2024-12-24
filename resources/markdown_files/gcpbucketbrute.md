### **Cloud/GCPBucketBrute/gcpbucketbrute.md**

# GCPBucketBrute

## Descripción

`GCPBucketBrute` es una herramienta diseñada para realizar ataques de fuerza bruta en buckets de Google Cloud Storage. Ayuda a identificar nombres de buckets expuestos y verificar su accesibilidad.

## Uso

```bash
gcpbucketbrute [opciones] <lista_buckets>
```

### Opciones principales

- `-p, --prefix prefijo`: Define un prefijo para los nombres de buckets.
- `-r, --regex patrón`: Utiliza una expresión regular para filtrar nombres.
- `-o, --output archivo`: Guarda los resultados en un archivo.
- `-t, --threads N`: Establece el número de hilos concurrentes.

## Ejemplos

- **Realizar fuerza bruta con una lista de nombres:**

  ```bash
  gcpbucketbrute -o encontrados.txt lista_buckets.txt
  ```

- **Usar un prefijo específico:**

  ```bash
  gcpbucketbrute -p miempresa- lista_buckets.txt
  ```

- **Ejecutar con múltiples hilos para mayor velocidad:**

  ```bash
  gcpbucketbrute -t 20 -o encontrados.txt lista_buckets.txt
  ```
