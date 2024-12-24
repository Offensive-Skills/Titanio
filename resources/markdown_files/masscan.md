### **Miscelánea/Escaneo y Enumeración/Masscan.md**

# Masscan

## Descripción

`Masscan` es una herramienta de escaneo de puertos extremadamente rápida que permite escanear grandes rangos de direcciones IP en busca de puertos abiertos. Su velocidad se debe a su diseño eficiente y capacidad para manejar un alto volumen de tráfico.

## Uso

```bash
masscan [opciones]
```

### Opciones principales

- `-p`: Especifica los puertos a escanear (e.g., `-p80,443` o `-p0-65535`).
- `-iL`: Archivo de entrada con listas de IPs.
- `-oL`: Archivo de salida en formato legible.
- `--rate`: Define la velocidad del escaneo (paquetes por segundo).
- `-sS`: Realiza un escaneo SYN.
- `-sU`: Escanea puertos UDP.
- `--banners`: Intenta capturar banners de servicios.
- `--open`: Muestra solo los puertos abiertos.

## Ejemplos

- Escanear los puertos 80 y 443 en una IP específica:
  
  ```bash
  masscan -p80,443 192.168.1.10
  ```

- Escanear todos los puertos en un rango de IPs con una velocidad de 10000 PPS:
  
  ```bash
  masscan -p0-65535 192.168.1.0/24 --rate=10000
  ```

- Escanear puertos TCP y UDP y guardar los resultados:
  
  ```bash
  masscan -p80,443,53 192.168.1.0/24 -sS -sU -oL resultados.txt
  ```

- Escanear y capturar banners de servicios:
  
  ```bash
  masscan -p80,443 192.168.1.10 --banners
  ```

