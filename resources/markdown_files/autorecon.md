### **Herramientas de Automatización/AutoRecon.md**

# AutoRecon

## Descripción

`AutoRecon` es una herramienta de automatización para la recolección de información y reconocimiento en pruebas de penetración. Combina múltiples herramientas de escaneo y enumeración para proporcionar un informe completo de la superficie de ataque de un objetivo.

## Uso

```bash
autorecon [opciones] objetivo
```

### Opciones principales

- `-t`: Define el número de hilos para el escaneo.
- `-o`: Especifica el directorio de salida para los informes.
- `--http`: Habilita el escaneo HTTP.
- `--ssh`: Habilita el escaneo SSH.
- `--exclude`: Excluye ciertos puertos o servicios del escaneo.

## Ejemplos

- Realizar un escaneo básico en un objetivo:

  ```bash
  autorecon -t 4 -o informes/ ejemplo.com
  ```

- Ejecutar AutoRecon excluyendo el puerto 80:

  ```bash
  autorecon -t 2 --exclude 80 -o informes/ ejemplo.com
  ```

- Habilitar escaneo HTTP y SSH:

  ```bash
  autorecon -t 4 --http --ssh -o informes/ ejemplo.com
  ```
