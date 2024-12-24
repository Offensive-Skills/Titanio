### **Cloud/Prowler/prowler.md**

# Prowler

## Descripción

`Prowler` es una herramienta de auditoría de seguridad para AWS que verifica configuraciones de seguridad y cumplimiento con estándares como CIS y GDPR. Genera informes detallados sobre hallazgos y recomendaciones.

## Uso

```bash
prowler [opciones]
```

### Opciones principales

- `-M, --mode`: Define el modo de ejecución (ejemplo: cis, security, custom).
- `-g, --groups`: Selecciona grupos de pruebas específicas.
- `-o, --output archivo`: Guarda el informe en un archivo.
- `-f, --format formato`: Especifica el formato del informe (text, json, html).

## Ejemplos

- **Ejecutar auditoría CIS y guardar el informe en HTML:**

  ```bash
  prowler -M cis -o informe_cis.html -f html
  ```

- **Realizar una auditoría de seguridad general:**

  ```bash
  prowler -M security
  ```

- **Guardar resultados en formato JSON:**

  ```bash
  prowler -o resultados.json -f json
  ```
