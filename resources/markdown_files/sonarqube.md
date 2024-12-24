### **Análisis de Código/SonarQube.md**

# SonarQube

## Descripción

`SonarQube` es una plataforma de código abierto para la inspección continua de la calidad del código. Analiza el código fuente en busca de bugs, vulnerabilidades y "code smells", proporcionando informes detallados y métricas para mejorar la calidad del software.

## Uso

```bash
sonar-scanner [opciones]
```

### Opciones principales

- `-Dsonar.projectKey`: Define la clave del proyecto.
- `-Dsonar.sources`: Especifica las fuentes del proyecto.
- `-Dsonar.host.url`: URL del servidor de SonarQube.
- `-Dsonar.login`: Token de autenticación.
- `-Dsonar.language`: Lenguaje de programación del proyecto.

## Ejemplos

- Ejecutar un análisis básico:

  ```bash
  sonar-scanner \
    -Dsonar.projectKey=mi_proyecto \
    -Dsonar.sources=. \
    -Dsonar.host.url=http://localhost:9000 \
    -Dsonar.login=mi_token
  ```

- Analizar un proyecto en Java:

  ```bash
  sonar-scanner \
    -Dsonar.projectKey=proyecto_java \
    -Dsonar.sources=src \
    -Dsonar.host.url=http://localhost:9000 \
    -Dsonar.login=mi_token \
    -Dsonar.language=java
  ```
