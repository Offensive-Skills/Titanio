### **Miscelánea/Recolección de Información/Shodan.md**

# Shodan

## Descripción

`Shodan` es un motor de búsqueda especializado en identificar dispositivos conectados a Internet. Permite a los usuarios encontrar información sobre servidores, dispositivos IoT, cámaras web, routers y más, basándose en servicios, puertos y banners detectados.

## Uso

```bash
shodan [comandos] [opciones]
```

### Comandos principales

- `init`: Inicializa la configuración con la API Key.
- `search`: Realiza búsquedas de dispositivos basadas en criterios específicos.
- `host`: Obtiene información detallada de un host específico.
- `scan`: Inicia un escaneo de una IP o rango de IPs.
- `download`: Descarga resultados de búsquedas guardadas.
- `info`: Muestra información sobre la cuenta y créditos.
- `--help`: Muestra ayuda y opciones disponibles.

### Opciones principales

- `--fields`: Especifica los campos a mostrar en los resultados.
- `--limit`: Define el número máximo de resultados a obtener.
- `--page`: Página de resultados a visualizar.
- `--pretty`: Formatea la salida para mayor legibilidad.

## Ejemplos

- Inicializar Shodan con una API Key:
  
  ```bash
  shodan init TU_API_KEY
  ```

- Buscar dispositivos con puerto SSH abierto:
  
  ```bash
  shodan search ssh
  ```

- Buscar cámaras web en un país específico:
  
  ```bash
  shodan search "webcam country:ES"
  ```

- Obtener información detallada de un host específico:
  
  ```bash
  shodan host 8.8.8.8
  ```

- Descargar los resultados de una búsqueda guardada:
  
  ```bash
  shodan download resultados.json "ssh"
  ```
