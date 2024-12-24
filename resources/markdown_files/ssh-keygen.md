### **Seguridad/SSH/ssh-keygen.md**

# ssh-keygen

## Descripción

`ssh-keygen` es una herramienta para generar, gestionar y convertir claves de autenticación para SSH (Secure Shell). Permite crear pares de claves públicas y privadas para autenticación sin contraseña y mejorar la seguridad en conexiones SSH.

## Uso

```bash
ssh-keygen [opciones]
```

### Opciones principales

- `-t tipo`: Especifica el tipo de clave (rsa, dsa, ecdsa, ed25519).
- `-b bits`: Define el tamaño en bits de la clave.
- `-f archivo`: Especifica el nombre de archivo para guardar la clave.
- `-N frase`: Establece una frase de contraseña para la clave.
- `-C comentario`: Añade un comentario a la clave.
- `-p`: Cambia la frase de contraseña de una clave existente.
- `-y`: Genera la clave pública a partir de una clave privada.

## Ejemplos

- Generar un par de claves RSA de 2048 bits:

  ```bash
  ssh-keygen -t rsa -b 2048 -f ~/.ssh/id_rsa
  ```

- Generar una clave ed25519 con comentario:

  ```bash
  ssh-keygen -t ed25519 -C "usuario@ejemplo.com"
  ```

- Cambiar la frase de contraseña de una clave existente:

  ```bash
  ssh-keygen -p -f ~/.ssh/id_rsa
  ```

- Obtener la clave pública de una clave privada:

  ```bash
  ssh-keygen -y -f ~/.ssh/id_rsa > id_rsa.pub
  ```
