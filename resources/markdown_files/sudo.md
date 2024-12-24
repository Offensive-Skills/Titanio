### **Básico/Miscelánea/sudo.md**

# sudo

## Descripción

`sudo` permite a un usuario ejecutar comandos con los privilegios de otro usuario, por defecto el superusuario.

## Uso

sudo [opciones] comando

### Opciones principales

- `-u`: Especifica el usuario con el que ejecutar el comando.
- `-s`: Inicia una shell con privilegios elevados.
- `-l`: Lista los permisos del usuario actual.
- `-k`: Borra el timestamp de autenticación.

## Ejemplos

- Ejecutar un comando como superusuario:

  sudo apt update

- Ejecutar un comando como otro usuario:

  sudo -u usuario comando

- Iniciar una shell como superusuario:

  sudo -s
