### **Básico/Miscelánea/kill.md**

# kill

## Descripción

`kill` envía señales a procesos, comúnmente usada para terminar procesos.

## Uso

kill [opciones] PID

### Opciones principales

- `-9`: Envia la señal SIGKILL para forzar la terminación.
- `-15`: Envía la señal SIGTERM (por defecto).
- `-l`: Lista todas las señales disponibles.

## Ejemplos

- Terminar un proceso con PID 1234:

  kill 1234

- Forzar la terminación de un proceso:

  kill -9 1234
