### **Explotación/Unix/unix_privesc_check.md**

# unix-privesc-check

## Descripción

`unix-privesc-check` es una herramienta de enumeración diseñada para identificar posibles vectores de escalada de privilegios en sistemas Unix y Linux. Analiza configuraciones, permisos de archivos, servicios en ejecución y otras configuraciones del sistema para detectar vulnerabilidades que podrían ser explotadas para obtener mayores privilegios.

## Uso

```bash
./unix-privesc-check.sh [opciones]
```

### Opciones principales

- `-h`: Muestra la ayuda y opciones disponibles.
- `--sudo`: Comprueba configuraciones relacionadas con sudo.
- `--ssh`: Verifica configuraciones de SSH.
- `--capabilities`: Revisa capacidades de archivos y procesos.
- `--audit`: Realiza una auditoría completa del sistema.

## Ejemplos

- Ejecutar una comprobación básica de escalada de privilegios:
  
  ```bash
  ./unix-privesc-check.sh
  ```

- Verificar configuraciones relacionadas con sudo:
  
  ```bash
  ./unix-privesc-check.sh --sudo
  ```

- Realizar una auditoría completa del sistema:
  
  ```bash
  ./unix-privesc-check.sh --audit
  ```
