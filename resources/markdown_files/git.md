### **Version_Control/Git/git.md**

# Git

## Descripción

`Git` es un sistema de control de versiones distribuido de código abierto diseñado para manejar proyectos de cualquier tamaño de manera eficiente. Permite a los desarrolladores rastrear cambios en el código fuente, colaborar en proyectos y gestionar versiones de manera efectiva.

## Uso

```bash
git [comando] [opciones]
```

### Comandos principales

- `git init`: Inicializa un nuevo repositorio Git en el directorio actual.
- `git clone [url]`: Clona un repositorio remoto en el directorio local.
- `git add [archivo]`: Añade cambios de un archivo específico al área de preparación (staging).
- `git commit -m "mensaje"`: Realiza un commit de los cambios preparados con un mensaje descriptivo.
- `git status`: Muestra el estado actual del repositorio, incluyendo cambios pendientes.
- `git push`: Envía los commits locales al repositorio remoto.
- `git pull`: Obtiene y fusiona cambios desde el repositorio remoto al local.
- `git branch`: Lista, crea o elimina ramas.
- `git merge [rama]`: Fusiona una rama específica en la rama actual.
- `git checkout [rama]`: Cambia a una rama específica.
- `git log`: Muestra el historial de commits.
- `git diff`: Muestra las diferencias entre cambios.
- `git reset`: Deshace cambios en el área de preparación o commits.

### Opciones comunes

- `-m "mensaje"`: Añade un mensaje al realizar un commit.
- `-b nombre_rama`: Crea y cambia a una nueva rama.
- `--hard`: Resetea el índice y el directorio de trabajo.
- `--soft`: Resetea el índice pero mantiene los cambios en el directorio de trabajo.
- `-a`: Añade automáticamente todos los archivos rastreados al commit.

## Ejemplos

- **Inicializar un nuevo repositorio Git:**

  ```bash
  git init
  ```

- **Clonar un repositorio remoto:**

  ```bash
  git clone https://github.com/usuario/repositorio.git
  ```

- **Añadir todos los cambios al área de preparación:**

  ```bash
  git add .
  ```

- **Realizar un commit con un mensaje descriptivo:**

  ```bash
  git commit -m "Añadir nueva funcionalidad de autenticación"
  ```

- **Ver el estado actual del repositorio:**

  ```bash
  git status
  ```

- **Enviar los commits locales al repositorio remoto:**

  ```bash
  git push origin main
  ```

- **Obtener y fusionar cambios desde el repositorio remoto:**

  ```bash
  git pull origin main
  ```

- **Crear y cambiar a una nueva rama llamada `feature-login`:**

  ```bash
  git checkout -b feature-login
  ```

- **Fusionar la rama `feature-login` en la rama `main`:**

  ```bash
  git checkout main
  git merge feature-login
  ```

- **Mostrar el historial de commits:**

  ```bash
  git log
  ```

- **Mostrar las diferencias entre cambios sin commitear:**

  ```bash
  git diff
  ```

- **Resetear el último commit manteniendo los cambios en el directorio de trabajo:**

  ```bash
  git reset --soft HEAD~1
  ```

- **Resetear el área de preparación y el directorio de trabajo al último commit:**

  ```bash
  git reset --hard HEAD
  ```
