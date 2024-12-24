### **Ingeniería Social/King Phisher.md**

# King Phisher

## Descripción

`King Phisher` es una herramienta de código abierto para simular campañas de phishing. Permite crear y gestionar campañas, rastrear interacciones de usuarios y analizar resultados para evaluar la susceptibilidad a ataques de ingeniería social.

## Uso

```bash
king-phisher [opciones]
```

### Opciones principales

- `-C CONFIG_FILE`: Especifica el archivo de configuración.
- `-f`: Ejecuta en modo frontend.
- `-s`: Ejecuta en modo servidor.
- `--no-ssl`: Desactiva SSL para conexiones.
- `--ssl-key`: Especifica la clave SSL.
- `--ssl-cert`: Especifica el certificado SSL.

## Ejemplos

- Iniciar King Phisher en modo servidor:

  ```bash
  king-phisher --no-ssl -C server_config.json
  ```

- Iniciar King Phisher en modo frontend conectado al servidor:

  ```bash
  king-phisher -C client_config.json
  ```

- Crear una nueva campaña de phishing:

  1. Abre King Phisher.
  2. Selecciona "New Campaign".
  3. Configura los detalles de la campaña, como el correo electrónico y la plantilla de phishing.
  4. Inicia la campaña y monitorea las interacciones.
