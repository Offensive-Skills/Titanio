### **Hacking Wi-Fi/Wifite.md**

# Wifite

## Descripción

`Wifite` es una herramienta de automatización para atacar redes Wi-Fi, enfocada en simplificar el proceso de cracking de contraseñas WEP y WPA. Integra múltiples herramientas como Aircrack-ng y Reaver para facilitar los ataques.

## Uso

```bash
wifite [opciones]
```

### Opciones principales

- `-i`: Especifica la interfaz de red.
- `-mac`: Clona direcciones MAC para evitar detección.
- `-wps`: Habilita ataques contra WPS.
- `-p`: Define el número de intentos de ataque.
- `--dict`: Especifica un diccionario para ataques de fuerza bruta.

## Ejemplos

- Iniciar Wifite con una interfaz específica:

  ```bash
  wifite -i wlan0mon
  ```

- Ejecutar ataques contra redes con WPS habilitado:

  ```bash
  wifite -i wlan0mon --wps
  ```

- Utilizar un diccionario personalizado para ataques de fuerza bruta:

  ```bash
  wifite -i wlan0mon --dict rockyou.txt
  ```
