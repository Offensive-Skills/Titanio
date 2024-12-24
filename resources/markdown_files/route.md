### **Básico/Utilidades de Red/route.md**

# route

## Descripción

`route` es una herramienta de red utilizada para mostrar y modificar la tabla de enrutamiento del sistema. Permite añadir, eliminar o cambiar rutas para dirigir el tráfico de red hacia diferentes destinos a través de interfaces específicas.

## Uso

```bash
route [opciones] [comando]
```

### Opciones principales

- `add`: Añade una nueva ruta a la tabla de enrutamiento.
- `del`: Elimina una ruta existente de la tabla de enrutamiento.
- `-net`: Especifica que la ruta es para una red.
- `-host`: Especifica que la ruta es para un host.
- `gw`: Define el gateway a utilizar para la ruta.
- `dev`: Especifica la interfaz de red para la ruta.
- `metric`: Define la métrica de la ruta, determinando la preferencia.

## Ejemplos

- Mostrar la tabla de enrutamiento actual:
  
  ```bash
  route -n
  ```

- Añadir una ruta estática para una red:
  
  ```bash
  route add -net 10.0.0.0/24 gw 192.168.1.1 dev eth0
  ```

- Añadir una ruta para un host específico:
  
  ```bash
  route add -host 192.168.1.100 gw 192.168.1.1 dev eth0
  ```

- Eliminar una ruta estática para una red:
  
  ```bash
  route del -net 10.0.0.0/24 gw 192.168.1.1 dev eth0
  ```

- Añadir una ruta con una métrica específica:
  
  ```bash
  route add -net 10.0.0.0/24 gw 192.168.1.1 dev eth0 metric 100
  ```