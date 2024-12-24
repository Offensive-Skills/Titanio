### **Herramientas de Seguridad/Cracking de Contraseñas/hydra.md**

# hydra

## Descripción

`hydra` es una herramienta de cracking de contraseñas de red rápida y flexible que soporta numerosos protocolos, incluyendo FTP, SSH, Telnet, SMTP, HTTP y muchos más. Se utiliza para probar la seguridad de servicios de autenticación remota.

## Uso

```bash
hydra [opciones] servidor servicio
```

### Opciones principales

- `-l usuario`: Especifica un único nombre de usuario.
- `-L archivo_usuarios`: Especifica un archivo con una lista de usuarios.
- `-p contraseña`: Especifica una única contraseña.
- `-P archivo_contraseñas`: Especifica un archivo con una lista de contraseñas.
- `-s puerto`: Especifica el puerto a utilizar.
- `-e nsr`: Prueba contraseñas vacías o el nombre de usuario como contraseña.
- `-t tareas`: Número de tareas paralelas (por defecto 16).
- `-o archivo_salida`: Especifica un archivo para guardar los resultados.

## Ejemplos

- Ataque de fuerza bruta contra SSH con un usuario específico:

  ```bash
  hydra -l usuario -P rockyou.txt ssh://ejemplo.com
  ```

- Ataque utilizando listas de usuarios y contraseñas contra FTP:

  ```bash
  hydra -L usuarios.txt -P contraseñas.txt ftp://192.168.1.1
  ```

- Especificar un puerto personalizado:

  ```bash
  hydra -l admin -P passwords.txt -s 2222 ssh://ejemplo.com
  ```

- Guardar resultados en un archivo:

  ```bash
  hydra -l usuario -P passwords.txt ssh://ejemplo.com -o resultados.txt
  ```
