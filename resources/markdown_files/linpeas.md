### **Herramientas de Seguridad/Enumeración/linpeas.md**

# linPEAS

## Descripción

`linPEAS` es un script de enumeración en Linux que busca posibles formas de escalada de privilegios en un sistema. Es utilizado por profesionales de seguridad para identificar configuraciones débiles y vulnerabilidades en sistemas Linux.

## Uso

Descargar el script y ejecutarlo en el sistema objetivo.

```bash
./linpeas.sh [opciones]
```

### Opciones principales

- `-a`: Ejecuta todas las comprobaciones, incluidas las más lentas.
- `-s`: Ejecuta un escaneo en modo sigiloso, minimizando el impacto.
- `-q`: Ejecuta en modo silencioso, sin colores ni formato.
- `-h`: Muestra la ayuda y opciones disponibles.

## Ejemplos

- Ejecutar linPEAS con comprobaciones estándar:

  ```bash
  ./linpeas.sh
  ```

- Ejecutar todas las comprobaciones:

  ```bash
  ./linpeas.sh -a
  ```

- Ejecutar en modo sigiloso:

  ```bash
  ./linpeas.sh -s
  ```
