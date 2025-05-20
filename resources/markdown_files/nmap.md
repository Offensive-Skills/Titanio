### **Básico/Utilidades de Red/nmap.md**

# nmap

## Descripción

`nmap` (Network Mapper) es una herramienta de seguridad y red utilizada para explorar redes y realizar auditorías de seguridad. Permite descubrir hosts y servicios en una red, identificando puertos abiertos, sistemas operativos y posibles vulnerabilidades.

## Uso

```bash
nmap [opciones] destino
```

### Opciones principales

- `-sS`: Realiza un escaneo SYN (stealth).
- `-sU`: Escanea puertos UDP.
- `-p`: Especifica los puertos a escanear.
- `-A`: Habilita la detección avanzada de versiones y sistemas operativos.
- `-O`: Detecta el sistema operativo del host.
- `-v`: Modo detallado, muestra información adicional durante el escaneo.
- `-Pn`: Omite el ping inicial y asume que el host está activo.
- `-T`: Define la velocidad del escaneo (0-5).

## Ejemplos

- Escanear los 1000 puertos más comunes en un host:
  
  ```bash
  nmap ejemplo.com
  ```

- Escanear puertos específicos:
  
  ```bash
  nmap -p 22,80,443 ejemplo.com
  ```

- Realizar un escaneo SYN stealth:
  
  ```bash
  nmap -sS ejemplo.com
  ```

- Escanear puertos UDP:
  
  ```bash
  nmap -sU ejemplo.com
  ```

- Detectar el sistema operativo y versiones de servicios:
  
  ```bash
  nmap -A ejemplo.com
  ```

- Escanear un rango de direcciones IP:
  
  ```bash
  nmap 192.168.1.1-50
  ```

- Escanear sin realizar ping inicial:
  
  ```bash
  nmap -Pn ejemplo.com
  ```

- Realizar un escaneo rápido con mayor velocidad:
  
  ```bash
  nmap -T4 ejemplo.com
  ```


---

Primer comando cuando nos enfrentamos a una máquina (Escaneamos todos los puertos para ver cuáles hay abiertos):
    ```
    sudo nmap -sS -p- --min-rate 5000 <IP>
    ```

Después de ver los puertos abiertos, los anotamos y ejecutamos el siguiente comando para hacer un escaneo exclusivo sobre ellos:
    ```
    nmap -p<puertos> -sCV --min-rate 5000 <IP>
    ```


