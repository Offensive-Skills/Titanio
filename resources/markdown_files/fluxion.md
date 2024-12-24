### **Wireless/Fluxion/fluxion.md**

# Fluxion

## Descripción

`Fluxion` es una herramienta de seguridad para redes Wi-Fi que combina ataques de desautenticación con técnicas de phishing para capturar contraseñas de redes protegidas. Utiliza un punto de acceso falso y una interfaz de phishing para engañar a los usuarios y obtener sus credenciales.

## Uso

```bash
sudo fluxion [opciones]
```

### Opciones principales

- `-i interfaz`: Selecciona la interfaz de red inalámbrica.
- `-a ESSID`: Define el ESSID de la red objetivo.
- `-c canal`: Especifica el canal de la red objetivo.
- `-p`: Configura el método de phishing a utilizar.
- `--help`: Muestra la ayuda y las opciones disponibles.

## Ejemplos

- Iniciar Fluxion con la interfaz wlan0:

  ```bash
  sudo fluxion -i wlan0
  ```

- Configurar el ESSID y canal de la red objetivo:

  ```bash
  sudo fluxion -a MiRed -c 6
  ```

- Seleccionar un método de phishing específico:

  ```bash
  sudo fluxion -p metodo1
  ```
