### **Version_Control/Subversion/subversion.md**

# Subversion (SVN)

## Descripción

`Subversion` (SVN) es un sistema de control de versiones centralizado de código abierto que permite a los desarrolladores gestionar y rastrear cambios en el código fuente de proyectos. Es utilizado para mantener un historial completo de modificaciones, facilitar la colaboración y asegurar la integridad del código.

## Uso

```bash
svn [comando] [opciones] [ruta]
```

### Comandos principales

- `svn checkout [URL]`: Clona un repositorio remoto en el directorio local.
- `svn update`: Actualiza el directorio de trabajo con los últimos cambios del repositorio.
- `svn commit -m "mensaje"`: Envía los cambios locales al repositorio con un mensaje descriptivo.
- `svn add [archivo]`: Añade un archivo o directorio al seguimiento de SVN.
- `svn delete [archivo]`: Elimina un archivo o directorio del repositorio.
- `svn status`: Muestra el estado de los archivos en el directorio de trabajo.
- `svn log`: Muestra el historial de commits del repositorio.
- `svn diff`: Muestra las diferencias entre los cambios locales y el repositorio.
- `svn merge [URL]`: Fusiona cambios desde una rama o etiqueta específica.
- `svn revert [archivo]`: Deshace cambios locales en un archivo específico.
- `svn info`: Muestra información detallada sobre el repositorio y el directorio de trabajo.

### Opciones comunes

- `-m "mensaje"`: Añade un mensaje al realizar un commit.
- `--username usuario`: Especifica el nombre de usuario para autenticarse.
- `--password contraseña`: Especifica la contraseña para autenticarse.
- `--force`: Fuerza la ejecución del comando incluso si hay conflictos.

## Ejemplos

- **Clonar un repositorio SVN:**

  ```bash
  svn checkout https://svn.ejemplo.com/repositorio/trunk proyecto
  ```

- **Actualizar el directorio de trabajo con los últimos cambios:**

  ```bash
  svn update
  ```

- **Añadir un nuevo archivo al repositorio:**

  ```bash
  svn add nuevo_archivo.py
  ```

- **Realizar un commit de cambios con un mensaje:**

  ```bash
  svn commit -m "Añadir nueva función de validación de usuarios"
  ```

- **Eliminar un archivo del repositorio:**

  ```bash
  svn delete archivo_obsoleto.txt
  svn commit -m "Eliminar archivo obsoleto"
  ```

- **Ver el estado de los archivos en el directorio de trabajo:**

  ```bash
  svn status
  ```

- **Mostrar el historial de commits:**

  ```bash
  svn log
  ```

- **Mostrar las diferencias entre cambios locales y el repositorio:**

  ```bash
  svn diff
  ```

- **Fusionar cambios desde una rama específica:**

  ```bash
  svn merge https://svn.ejemplo.com/repositorio/branches/nueva_rama
  ```

- **Revertir cambios locales en un archivo específico:**

  ```bash
  svn revert archivo_modificado.py
  ```

- **Obtener información detallada sobre el repositorio:**

  ```bash
  svn info
  ```

- **Realizar un commit con autenticación específica:**

  ```bash
  svn commit -m "Actualizar documentación" --username usuario --password contraseña
  ```

- **Forzar la adición de un archivo ya existente en el repositorio:**

  ```bash
  svn add archivo_existente.py --force
  ```
