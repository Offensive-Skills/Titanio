### **Hacking Web/Explotación de Sesiones/Cookie Cadger.md**

# Cookie Cadger

## Descripción

`Cookie Cadger` es una herramienta de análisis de sesiones web que captura y analiza cookies de usuarios para identificar vulnerabilidades relacionadas con la gestión de sesiones. Permite detectar problemas como cookies sin cifrar, uso de cookies predecibles y otros riesgos asociados.

## Uso

```bash
cookie_cadger [opciones]
```

### Opciones principales

- `-i`: Especifica la interfaz de red a usar para capturar tráfico.
- `-p`: Define el puerto del proxy.
- `-o`: Define el archivo de salida para guardar las cookies capturadas.
- `--ignore-ssl`: Ignora la verificación SSL para capturar tráfico HTTPS.
- `-h`: Muestra ayuda y opciones disponibles.

## Ejemplos

- Iniciar Cookie Cadger en la interfaz eth0 y guardar las cookies en un archivo:

  ```bash
  cookie_cadger -i eth0 -o cookies.txt
  ```

- Capturar tráfico HTTPS ignorando la verificación SSL:

  ```bash
  cookie_cadger -i eth0 --ignore-ssl
  ```

- Iniciar Cookie Cadger con un proxy en el puerto 8080:

  ```bash
  cookie_cadger -p 8080
  ```
