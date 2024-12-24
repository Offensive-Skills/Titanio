### **Version_Control/GitTools/gittools.md**

# GitTools

## Descripción

`GitTools` es un conjunto de herramientas diseñadas para automatizar y mejorar la gestión de repositorios Git. Incluye utilidades para análisis de seguridad, extracción de información, gestión de ramas y optimización de flujos de trabajo, facilitando el manejo eficiente de proyectos con Git.

## Uso

Cada herramienta dentro de `GitTools` tiene su propio comando y conjunto de opciones. A continuación se presentan algunas de las herramientas más comunes:

### Comandos principales

- `git-secrets`: Evita la inclusión de credenciales sensibles en los commits.
- `git-fuzzy`: Facilita la navegación rápida por el historial de commits.
- `git-town`: Mejora la gestión de ramas y la integración continua.
- `git-filter-repo`: Reescribe el historial de un repositorio Git de manera eficiente.
- `git-extras`: Añade comandos útiles adicionales a Git.
- `git-quick-stats`: Genera estadísticas rápidas sobre el repositorio.
- `git-delta`: Mejora la visualización de diferencias en Git.

### Opciones comunes

Las opciones varían según la herramienta específica. A continuación se muestran ejemplos para algunas de las herramientas mencionadas:

#### **git-secrets**

- `--install`: Instala `git-secrets` en el repositorio actual.
- `--register-aws`: Añade reglas para evitar la inclusión de claves AWS.
- `--scan`: Escanea el historial del repositorio en busca de credenciales.

#### **git-filter-repo**

- `--path ruta`: Filtra el historial para incluir solo el camino especificado.
- `--invert-paths`: Excluye el camino especificado del historial.
- `--replace-text archivo`: Reemplaza texto específico en el historial.

## Ejemplos

### **git-secrets**

- **Instalar `git-secrets` en el repositorio actual:**

  ```bash
  git secrets --install
  ```

- **Registrar reglas para evitar la inclusión de claves AWS:**

  ```bash
  git secrets --register-aws
  ```

- **Escanear el historial en busca de credenciales:**

  ```bash
  git secrets --scan
  ```

### **git-filter-repo**

- **Filtrar el historial para incluir solo la carpeta `src`:**

  ```bash
  git filter-repo --path src/ --force
  ```

- **Excluir la carpeta `docs` del historial:**

  ```bash
  git filter-repo --invert-paths --path docs/ --force
  ```

- **Reemplazar texto sensible en todo el historial:**

  ```bash
  git filter-repo --replace-text reemplazos.txt --force
  ```

### **git-extras**

- **Crear un log gráfico de commits:**

  ```bash
  git summary
  ```

- **Mostrar información de las ramas activas:**

  ```bash
  git branches
  ```

- **Generar estadísticas rápidas del repositorio:**

  ```bash
  git quick-stats
  ```

### **git-delta**

- **Utilizar `delta` como el visualizador de diferencias por defecto:**

  ```bash
  git config --global core.pager delta
  ```

- **Mostrar diferencias con resaltado de sintaxis mejorado:**

  ```bash
  git diff | delta
  ```

- **Configurar `delta` para colores personalizados:**

  ```bash
  git config --global delta.color-added "green bold"
  git config --global delta.color-removed "red bold"
  ```

## Instalación

La instalación de `GitTools` varía según la herramienta específica. A continuación se muestra cómo instalar algunas de las herramientas más comunes:

- **git-secrets:**

  ```bash
  brew install git-secrets
  ```

- **git-filter-repo:**

  ```bash
  pip install git-filter-repo
  ```

- **git-extras:**

  ```bash
  brew install git-extras
  ```

- **git-delta:**

  ```bash
  brew install git-delta
  ```
