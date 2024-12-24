### **Herramientas de Red/nbtscan/nbtscan.md**

# nbtscan

## Descripción

`nbtscan` es una herramienta de escaneo de redes que busca información NetBIOS en redes IP. Permite obtener nombres de host, grupos de trabajo y direcciones MAC de dispositivos Windows.

## Uso

```bash
nbtscan [opciones] rango
```

### Opciones principales

- `-r`: Muestra el nombre de usuario registrado.
- `-v`: Modo detallado.
- `-h`: Muestra la ayuda.
- `-s`: Especifica el separador de campos en la salida.

## Ejemplos

- Escanear una red completa:

  ```bash
  nbtscan 192.168.1.0/24
  ```

- Escanear un rango específico:

  ```bash
  nbtscan 192.168.1.1-192.168.1.50
  ```

- Modo detallado:

  ```bash
  nbtscan -v 192.168.1.0/24
  ```

