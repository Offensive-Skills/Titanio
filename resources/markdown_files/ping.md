### **Básico/Utilidades de Red/ping.md**

# ping

## Descripción

`ping` es una herramienta de red utilizada para verificar la conectividad entre el equipo local y otro host en una red. Envía paquetes ICMP de eco y mide el tiempo que tardan en recibir una respuesta, lo que ayuda a diagnosticar problemas de red.

## Uso

```bash
ping [opciones] destino
```

### Opciones principales

- `-c`: Especifica el número de paquetes a enviar.
- `-i`: Define el intervalo entre envíos de paquetes.
- `-t`: Establece el tiempo de vida (TTL) de los paquetes.
- `-s`: Define el tamaño de los paquetes en bytes.
- `-W`: Establece el tiempo de espera en segundos para una respuesta.
- `-q`: Modo silencioso, muestra solo el resumen al final.
- `-4`: Fuerza el uso de IPv4.
- `-6`: Fuerza el uso de IPv6.

## Ejemplos

- Enviar 4 paquetes a un host:
  
  ```bash
  ping -c 4 ejemplo.com
  ```

- Enviar paquetes con un tamaño de 100 bytes:
  
  ```bash
  ping -s 100 ejemplo.com
  ```

- Establecer el intervalo entre paquetes a 2 segundos:
  
  ```bash
  ping -i 2 ejemplo.com
  ```

- Mostrar solo el resumen de la prueba:
  
  ```bash
  ping -c 4 -q ejemplo.com
  ```

- Forzar el uso de IPv6:
  
  ```bash
  ping -6 ejemplo.com
  ```
