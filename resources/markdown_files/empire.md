### **Post-Explotación/Frameworks/Empire.md**

# Empire

## Descripción

**Empire** es un framework de post-explotación que permite ejecutar agentes en sistemas Windows, macOS y Linux. Proporciona una interfaz para controlar sistemas comprometidos y ejecutar módulos para tareas de post-explotación.

## Uso

Iniciar el servidor Empire y utilizar la interfaz de línea de comandos.

```bash
./empire
```

### Opciones principales

- **Listeners**: Configura escuchas para recibir conexiones de agentes.
- **Agents**: Lista y gestiona agentes conectados.
- **Modules**: Ejecuta módulos de post-explotación.

## Ejemplos

- Crear un listener:

  ```bash
  listeners
  uselistener http
  set Name myListener
  execute
  ```

- Generar un stager:

  ```bash
  usestager windows/launcher_bat
  set Listener myListener
  generate
  ```

