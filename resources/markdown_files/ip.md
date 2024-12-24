### **Básico/Utilidades de Red/ip.md**

# ip

## Descripción

`ip` es una herramienta de red moderna y versátil utilizada para configurar y mostrar información sobre interfaces de red, direcciones IP, rutas y túneles. Reemplaza en gran medida a `ifconfig` y `netstat`, ofreciendo funcionalidades más avanzadas y flexibles.

## Uso

```bash
ip [comando] [opciones]
```

### Comandos principales

- `addr`: Gestiona direcciones IP.
- `link`: Gestiona enlaces de red.
- `route`: Gestiona rutas de enrutamiento.
- `neigh`: Gestiona vecinos ARP.
- `rule`: Gestiona reglas de enrutamiento.
- `monitor`: Monitorea eventos de red en tiempo real.

### Opciones principales

- `add`: Añade una dirección, ruta o enlace.
- `del`: Elimina una dirección, ruta o enlace.
- `show`: Muestra la configuración actual.
- `flush`: Limpia direcciones, rutas o vecinos.
- `change`: Modifica la configuración existente.

## Ejemplos

- Mostrar todas las direcciones IP:
  
  ```bash
  ip addr show
  ```

- Asignar una dirección IP a una interfaz:
  
  ```bash
  ip addr add 192.168.1.10/24 dev eth0
  ```

- Eliminar una dirección IP de una interfaz:
  
  ```bash
  ip addr del 192.168.1.10/24 dev eth0
  ```

- Activar una interfaz de red:
  
  ```bash
  ip link set eth0 up
  ```

- Desactivar una interfaz de red:
  
  ```bash
  ip link set eth0 down
  ```

- Mostrar la tabla de enrutamiento:
  
  ```bash
  ip route show
  ```

- Añadir una ruta estática:
  
  ```bash
  ip route add 10.0.0.0/24 via 192.168.1.1
  ```

- Eliminar una ruta estática:
  
  ```bash
  ip route del 10.0.0.0/24 via 192.168.1.1
  ```

- Monitorear eventos de red en tiempo real:
  
  ```bash
  ip monitor
  ```