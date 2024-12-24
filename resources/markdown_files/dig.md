### **Básico/Utilidades de Red/dig.md**

# dig

## Descripción

`dig` (Domain Information Groper) es una herramienta de red avanzada utilizada para realizar consultas DNS detalladas. Proporciona información detallada sobre los registros DNS de un dominio, lo que facilita la resolución de problemas y el análisis de configuraciones DNS.

## Uso

```bash
dig [opciones] [nombre] [tipo]
```

### Opciones principales

- `@servidor`: Especifica el servidor DNS a utilizar para la consulta.
- `+short`: Muestra una salida breve y concisa.
- `+verbose`: Muestra información detallada sobre la consulta.
- `+nocmd`: Omite la impresión del comando ejecutado.
- `+noall`: No muestra ninguna sección por defecto.
- `+answer`: Muestra solo la sección de respuestas.
- `+additional`: Incluye la sección adicional en la salida.
- `+time`: Define el tiempo de espera en segundos para una respuesta.
- `+tries`: Establece el número de intentos en caso de no recibir respuesta.

## Ejemplos

- Consultar la dirección IP de un dominio:
  
  ```bash
  dig ejemplo.com A
  ```

- Consultar registros MX de un dominio:
  
  ```bash
  dig ejemplo.com MX
  ```

- Usar un servidor DNS específico para la consulta:
  
  ```bash
  dig @8.8.8.8 ejemplo.com
  ```

- Mostrar solo la respuesta de la consulta:
  
  ```bash
  dig ejemplo.com A +short
  ```

- Realizar una consulta detallada:
  
  ```bash
  dig ejemplo.com A +verbose
  ```

- Definir un tiempo de espera de 5 segundos:
  
  ```bash
  dig ejemplo.com A +time=5
  ```