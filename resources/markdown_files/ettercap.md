### **Análisis de Tráfico Web/Ettercap.md**

# Ettercap

## Descripción

`Ettercap` es una herramienta de sniffing y análisis de tráfico de red enfocada en ataques de tipo Man-in-the-Middle (MITM). Permite interceptar, modificar y registrar el tráfico de red en tiempo real, ofreciendo funcionalidades para la detección de vulnerabilidades y análisis de seguridad.

## Uso

```bash
ettercap [opciones]
```

### Opciones principales

- `-G`: Inicia Ettercap con la interfaz gráfica.
- `-T`: Modo texto, útil para servidores sin interfaz gráfica.
- `-M`: Define el tipo de ataque MITM a realizar.
- `-i`: Especifica la interfaz de red a utilizar.
- `-q`: Modo silencioso, sin salida detallada.
- `-P`: Especifica el plugin de Ettercap a usar.
- `-F`: Define un archivo de filtros para modificar el tráfico.

## Ejemplos

- Iniciar Ettercap en modo gráfico:

  ```bash
  ettercap -G
  ```

- Iniciar Ettercap en modo texto e interceptar tráfico ARP:

  ```bash
  ettercap -T -M arp:remote /192.168.1.10// /192.168.1.20//
  ```

- Usar un archivo de filtros para modificar el tráfico:

  ```bash
  ettercap -T -F filtros.ef
  ```

- Especificar la interfaz de red eth0:

  ```bash
  ettercap -T -i eth0 -M arp /192.168.1.0/24//
  ```
