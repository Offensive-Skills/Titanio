### **Wireless/Wifiphisher/wifiphisher.md**

# Wifiphisher

## Descripción

`Wifiphisher` es una herramienta de phishing de redes Wi-Fi que automatiza ataques de ingeniería social para engañar a los usuarios y obtener sus credenciales de red. Utiliza ataques de phishing de redireccionamiento para crear puntos de acceso falsos que imitan redes legítimas.

## Uso

```bash
sudo wifiphisher [opciones]
```

### Opciones principales

- `-a`: Selecciona el método de ataque.
- `-e ESSID`: Define el ESSID de la red falsa.
- `-p`: Configura el canal de la red falsa.
- `--no-deauth`: Evita el envío de paquetes de deautenticación.
- `--essids`: Lista las ESSIDs disponibles para atacar.
- `-h`: Muestra la ayuda y opciones disponibles.

## Ejemplos

- Iniciar un ataque básico de phishing:

  ```bash
  sudo wifiphisher
  ```

- Seleccionar un ESSID específico para imitar:

  ```bash
  sudo wifiphisher -e MiRedFalsa
  ```

- Configurar el canal de la red falsa:

  ```bash
  sudo wifiphisher -p 6
  ```

- Listar las ESSIDs disponibles para atacar:

  ```bash
  sudo wifiphisher --essids
  ```
