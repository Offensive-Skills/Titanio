### **Básico/Transferencia de Archivos/rsync.md**

# rsync

## Descripción

`rsync` es una herramienta para sincronizar y transferir archivos de forma eficiente entre sistemas locales o remotos.

## Uso

rsync [opciones] origen destino

### Opciones principales

- `-a`: Modo archivo, equivalente a `-rlptgoD`.
- `-v`: Modo detallado.
- `-z`: Comprime archivos durante la transferencia.
- `-P`: Muestra el progreso y reanuda transferencias interrumpidas.
- `-r`: Copia directorios de forma recursiva.
- `--delete`: Elimina en destino los archivos que ya no existen en origen.

## Ejemplos

- Sincronizar directorios localmente:

  rsync -av carpeta_origen/ carpeta_destino/

- Sincronizar con un servidor remoto:

  rsync -avz carpeta/ usuario@servidor:/ruta/destino/

- Sincronizar y eliminar archivos obsoletos en el destino:

  rsync -av --delete carpeta_origen/ carpeta_destino/

- Mostrar el progreso durante la transferencia:

  rsync -avP archivo usuario@servidor:/ruta/destino/

Estos son los archivos solicitados siguiendo el formato especificado. Cada herramienta se presenta una tras otra, sin cajas de código ni líneas separadoras, para facilitar una consulta rápida y efectiva.
