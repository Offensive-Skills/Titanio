### **Cloud/Pacu/pacu.md**

# Pacu

## Descripción

`Pacu` es un marco de explotación de AWS de código abierto utilizado para pruebas de penetración y evaluación de seguridad en entornos de Amazon Web Services. Permite identificar y explotar vulnerabilidades en configuraciones de AWS.

## Uso

```bash
pacu
```

### Comandos principales

- `help`: Muestra la ayuda y los comandos disponibles.
- `use <módulo>`: Carga un módulo específico para su ejecución.
- `run <módulo>`: Ejecuta el módulo cargado.
- `list`: Lista todos los módulos disponibles.

## Ejemplos

- **Iniciar Pacu y listar módulos:**

  ```bash
  pacu
  > list
  ```

- **Cargar y ejecutar el módulo de enumeración de S3:**

  ```bash
  pacu
  > use s3_enum
  > run
  ```

- **Ejecutar el módulo de enumeración de IAM:**

  ```bash
  pacu
  > use iam_enum
  > run
