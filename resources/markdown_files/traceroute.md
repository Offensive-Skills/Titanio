### **Básico/Utilidades de Red/traceroute.md**

# traceroute

## Descripción

`traceroute` es una herramienta de red utilizada para rastrear la ruta que siguen los paquetes desde el host local hasta un destino específico en una red. Muestra cada salto intermedio y el tiempo que tarda cada uno, lo que ayuda a identificar dónde pueden estar ocurriendo problemas de conectividad.

## Uso

```bash
traceroute [opciones] destino
```

### Opciones principales

- `-m`: Establece el número máximo de saltos.
- `-n`: Muestra direcciones IP en lugar de nombres de dominio.
- `-w`: Define el tiempo de espera en segundos para cada respuesta.
- `-q`: Especifica el número de paquetes por salto.
- `-I`: Usa paquetes ICMP ECHO en lugar de paquetes UDP.
- `-T`: Usa paquetes TCP SYN en lugar de paquetes UDP.

## Ejemplos

- Rastrear la ruta a un dominio:
  
  ```bash
  traceroute ejemplo.com
  ```

- Rastrear la ruta usando ICMP ECHO:
  
  ```bash
  traceroute -I ejemplo.com
  ```

- Rastrear la ruta sin resolver nombres de dominio:
  
  ```bash
  traceroute -n ejemplo.com
  ```

- Establecer un máximo de 20 saltos:
  
  ```bash
  traceroute -m 20 ejemplo.com
  ```

- Definir un tiempo de espera de 5 segundos por respuesta:
  
  ```bash
  traceroute -w 5 ejemplo.com
  ```

- Usar paquetes TCP SYN para el rastreo:
  
  ```bash
  traceroute -T ejemplo.com
  ```