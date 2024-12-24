### **Básico/Utilidades de Red/netstat.md**

# netstat

## Descripción

`netstat` es una herramienta de red utilizada para mostrar información sobre las conexiones de red, tablas de enrutamiento, estadísticas de interfaces y más. Es útil para diagnosticar problemas de red y monitorear el estado de las conexiones.

## Uso

```bash
netstat [opciones]
```

### Opciones principales

- `-a`: Muestra todas las conexiones y puertos de escucha.
- `-t`: Muestra conexiones TCP.
- `-u`: Muestra conexiones UDP.
- `-l`: Muestra solo puertos en escucha.
- `-n`: Muestra direcciones y puertos en formato numérico.
- `-p`: Muestra el identificador de proceso y el nombre del programa.
- `-r`: Muestra la tabla de enrutamiento.
- `-i`: Muestra estadísticas de interfaces.
- `-s`: Muestra estadísticas por protocolo.

## Ejemplos

- Mostrar todas las conexiones y puertos en escucha:
  
  ```bash
  netstat -a
  ```

- Mostrar solo conexiones TCP:
  
  ```bash
  netstat -t
  ```

- Mostrar conexiones UDP en formato numérico:
  
  ```bash
  netstat -un
  ```

- Mostrar la tabla de enrutamiento:
  
  ```bash
  netstat -r
  ```

- Mostrar estadísticas de interfaces:
  
  ```bash
  netstat -i
  ```

- Mostrar conexiones junto con el proceso asociado:
  
  ```bash
  netstat -p
  ```

- Mostrar estadísticas por protocolo:
  
  ```bash
  netstat -s
  ```