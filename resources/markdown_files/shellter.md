### **Explotación/Evasión Antivirus/Shellter.md**

# Shellter

## Descripción

**Shellter** es una herramienta dinámica de inyección de shellcode para Windows. Permite inyectar código malicioso en aplicaciones Windows legítimas para crear ejecutables que puedan evadir la detección de antivirus.

## Uso

```cmd
shellter.exe
```

La herramienta es interactiva y guía al usuario a través del proceso.

### Opciones principales

- **Modo automático (A)**: La herramienta selecciona automáticamente las opciones.
- **Modo manual (M)**: El usuario define las opciones y configuraciones.
- **Seleccionar ejecutable**: Especifica el archivo en el que se inyectará el shellcode.
- **Seleccionar payload**: Elige el shellcode a inyectar.

## Ejemplos

- Iniciar Shellter en modo automático:

  ```cmd
  shellter.exe
  ```

  Luego, seguir las instrucciones en pantalla.

