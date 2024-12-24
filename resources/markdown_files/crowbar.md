### **PowerShell/Crowbar/crowbar.md**

# Crowbar

## Descripción

`Crowbar` es una herramienta de fuerza bruta diseñada para realizar ataques a servicios de autenticación, como SSH, RDP, y servicios web. Es eficiente en la identificación de credenciales válidas mediante el uso de diccionarios y técnicas de automatización, facilitando las pruebas de penetración y auditorías de seguridad.

## Uso

```bash
crowbar [opciones]
```

### Opciones principales

- `-b`: Define el servicio objetivo (e.g., ssh, rdp).
- `-t TARGET`: Especifica la dirección IP o nombre del host objetivo.
- `-U USERLIST`: Lista de usuarios a probar.
- `-P PASSLIST`: Lista de contraseñas a probar.
- `--threads NUM`: Establece el número de hilos concurrentes.
- `--timeout SEG`: Define el tiempo de espera para las conexiones.
- `--verbose`: Activa el modo detallado.

## Ejemplos

- Realizar un ataque de fuerza bruta a SSH:
  
  ```bash
  crowbar -b ssh -t 192.168.1.100 -U usuarios.txt -P contraseñas.txt
  ```

- Ataque a RDP con múltiples hilos:
  
  ```bash
  crowbar -b rdp -t 192.168.1.100 -U usuarios.txt -P contraseñas.txt --threads 50
  ```

- Ataque a un servicio web con tiempo de espera personalizado:
  
  ```bash
  crowbar -b http -t ejemplo.com -U usuarios.txt -P contraseñas.txt --timeout 10
  ```

- Ejecutar en modo verbose para obtener más detalles:
  
  ```bash
  crowbar -b ssh -t 192.168.1.100 -U usuarios.txt -P contraseñas.txt --verbose
  ```

