### **Miscelánea/Escaneo y Enumeración/Unicornscan.md**

# Unicornscan

## Descripción

`Unicornscan` es una herramienta de escaneo de red diseñada para realizar enumeraciones detalladas de puertos y servicios. Se enfoca en la recopilación de información a nivel de red con alta precisión y eficiencia, siendo útil para pruebas de penetración y auditorías de seguridad.

## Uso

```bash
unicornscan [opciones]
```

### Opciones principales

- `-i`: Interfaz de red a utilizar.
- `-p`: Especifica los puertos a escanear.
- `-c`: Configura el tipo de escaneo (e.g., TCP, UDP).
- `-m`: Define el modo de ejecución.
- `-o`: Archivo de salida para los resultados.
- `-t`: Tiempo de espera para las respuestas.
- `-r`: Define la velocidad del escaneo.

## Ejemplos

- Escanear puertos TCP 80 y 443 en una IP específica:
  
  ```bash
  unicornscan -i eth0 -p 80,443 192.168.1.10
  ```

- Escanear un rango de puertos en múltiples IPs y guardar los resultados:
  
  ```bash
  unicornscan -i eth0 -p 1-1000 192.168.1.0/24 -o resultados.txt
  ```

- Realizar un escaneo UDP en una IP específica:
  
  ```bash
  unicornscan -i eth0 -p U:53,161 192.168.1.10
  ```

- Configurar un escaneo detallado con modos específicos:
  
  ```bash
  unicornscan -i eth0 -p 22,80,443 -mT:3 -oA detalle 192.168.1.10
  ```
