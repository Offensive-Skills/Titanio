### **Version_Control/Mercurial/mercurial.md**

# Mercurial

## Descripción

`Mercurial` es un sistema de control de versiones distribuido de código abierto diseñado para manejar proyectos de cualquier tamaño con eficiencia. Ofrece herramientas potentes para rastrear cambios, gestionar ramas y facilitar la colaboración entre desarrolladores, manteniendo un historial completo de versiones.

## Uso

```bash
hg [comando] [opciones]
```

### Comandos principales

- `hg init`: Inicializa un nuevo repositorio Mercurial en el directorio actual.
- `hg clone [URL]`: Clona un repositorio remoto en el directorio local.
- `hg add [archivo]`: Añade un archivo o directorio al seguimiento de Mercurial.
- `hg commit -m "mensaje"`: Realiza un commit de los cambios con un mensaje descriptivo.
- `hg status`: Muestra el estado actual del repositorio, incluyendo cambios pendientes.
- `hg push`: Envía los commits locales al repositorio remoto.
- `hg pull`: Obtiene cambios desde el repositorio remoto al local.
- `hg update [revision]`: Cambia a una revisión específica del repositorio.
- `hg log`: Muestra el historial de commits.
- `hg diff`: Muestra las diferencias entre cambios.
- `hg branch [nombre_rama]`: Crea y cambia a una nueva rama.
- `hg merge [rama]`: Fusiona una rama específica en la rama actual.

### Opciones comunes

- `-m "mensaje"`: Añade un mensaje al realizar un commit.
- `-u usuario`: Especifica el nombre de usuario para autenticarse.
- `--debug`: Modo de depuración, muestra información adicional.
- `-r`: Define la revisión específica para comandos como `update` o `diff`.

## Ejemplos

- **Inicializar un nuevo repositorio Mercurial:**

  ```bash
  hg init
  ```

- **Clonar un repositorio remoto:**

  ```bash
  hg clone https://hg.ejemplo.com/repositorio proyecto
  ```

- **Añadir un nuevo archivo al repositorio:**

  ```bash
  hg add nuevo_archivo.py
  ```

- **Realizar un commit con un mensaje descriptivo:**

  ```bash
  hg commit -m "Añadir nueva función de autenticación"
  ```

- **Ver el estado actual del repositorio:**

  ```bash
  hg status
  ```

- **Enviar los commits locales al repositorio remoto:**

  ```bash
  hg push
  ```

- **Obtener y fusionar cambios desde el repositorio remoto:**

  ```bash
  hg pull
  hg update
  ```

- **Crear y cambiar a una nueva rama llamada `feature-login`:**

  ```bash
  hg branch feature-login
  ```

- **Fusionar la rama `feature-login` en la rama principal:**

  ```bash
  hg update default
  hg merge feature-login
  hg commit -m "Fusionar feature-login en default"
  ```

- **Mostrar el historial de commits:**

  ```bash
  hg log
  ```

- **Mostrar las diferencias entre cambios sin commitear:**

  ```bash
  hg diff
  ```

- **Actualizar a una revisión específica:**

  ```bash
  hg update -r 10
  ```

- **Realizar un commit con un usuario específico:**

  ```bash
  hg commit -m "Actualizar documentación" -u usuario
  ```

- **Ejecutar Mercurial en modo de depuración:**

  ```bash
  hg --debug status
  ```
