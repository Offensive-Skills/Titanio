### **Herramientas de Seguridad/Enumeración/suid3num.md**

# SUID3NUM

## Descripción

`SUID3NUM` es una herramienta que ayuda a identificar binarios SUID con permisos inseguros en sistemas Linux. Busca binarios SUID y analiza su potencial para ser explotados para escalada de privilegios.

## Uso

```bash
./suid3num.py [opciones]
```

### Opciones principales

- `-e`: Ejecuta comprobaciones exhaustivas en cada binario SUID.
- `-l`: Genera un log detallado de los resultados.
- `-h`: Muestra la ayuda y opciones disponibles.

## Ejemplos

- Ejecutar análisis estándar:

  ```bash
  ./suid3num.py
  ```

- Ejecutar comprobaciones exhaustivas:

  ```bash
  ./suid3num.py -e
  ```

- Generar un log de resultados:

  ```bash
  ./suid3num.py -l
  ```

