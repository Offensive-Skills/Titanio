### **Básico/Utilidades de Red/nslookup.md**

# nslookup

## Descripción

`nslookup` es una herramienta de red utilizada para consultar servidores DNS y obtener información sobre nombres de dominio, como direcciones IP, registros MX y otros tipos de registros DNS.

## Uso

```bash
nslookup [opciones] [nombre]
```

### Opciones principales

- `-type`: Especifica el tipo de registro DNS a consultar (e.g., A, MX, NS).
- `-debug`: Muestra información de depuración detallada.
- `-timeout`: Define el tiempo de espera en segundos para una respuesta.
- `-retry`: Establece el número de intentos en caso de no recibir respuesta.
- `servidor`: Especifica el servidor DNS a utilizar para la consulta.

## Ejemplos

- Consultar la dirección IP de un dominio:
  
  ```bash
  nslookup ejemplo.com
  ```

- Consultar registros MX de un dominio:
  
  ```bash
  nslookup -type=MX ejemplo.com
  ```

- Usar un servidor DNS específico para la consulta:
  
  ```bash
  nslookup ejemplo.com 8.8.8.8
  ```

- Mostrar información detallada de la consulta:
  
  ```bash
  nslookup -debug ejemplo.com
  ```

- Establecer un tiempo de espera de 5 segundos:
  
  ```bash
  nslookup -timeout=5 ejemplo.com
  ```