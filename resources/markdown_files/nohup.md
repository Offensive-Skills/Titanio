### **Básico/Miscelánea/nohup.md**

# nohup

## Descripción

`nohup` ejecuta un comando ignorando la señal SIGHUP, permitiendo que continúe ejecutándose después de cerrar la sesión.

## Uso

nohup comando [argumentos] &

## Ejemplos

- Ejecutar un script y mantenerlo activo:

  nohup ./script.sh &

- Ejecutar un comando y redirigir la salida:

  nohup comando > salida.log 2>&1 &
