### **Explotación/Evasión Antivirus/Veil_Evasion.md**

# Veil-Evasion

## Descripción

**Veil-Evasion** es una herramienta diseñada para generar payloads que evaden la detección de software antivirus. Permite a los profesionales de seguridad probar la eficacia de soluciones antivirus y mejorar la seguridad.

## Uso

```bash
veil-evasion
```

Luego, se sigue el menú interactivo para generar el payload deseado.

### Opciones principales

- **Listar payloads disponibles**: Muestra los payloads que se pueden generar.
- **Configurar opciones del payload**: Establece parámetros como `LHOST` y `LPORT`.
- **Seleccionar método de evasión**: Elige técnicas para evitar detección.

## Ejemplos

- Iniciar Veil-Evasion:

  ```bash
  veil-evasion
  ```

- Listar payloads:

  ```bash
  use python
  list
  ```

- Generar un payload con opciones personalizadas:

  ```bash
  set LHOST 192.168.1.100
  set LPORT 4444
  generate
  ```
