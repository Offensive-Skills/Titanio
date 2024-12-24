### **Post-Explotación/Frameworks/Covenant.md**

# Covenant

## Descripción

**Covenant** es un framework de comando y control (C2) que proporciona capacidades de post-explotación para pruebas de penetración. Ofrece una interfaz web para gestionar agentes en sistemas comprometidos.

## Uso

Iniciar el servidor Covenant y acceder a la interfaz web.

```bash
dotnet Covenant.dll
```

### Opciones principales

- **Listeners**: Configura listeners para recibir conexiones.
- **Grunts**: Agentes que se ejecutan en los sistemas objetivos.
- **Tasks**: Comandos y módulos que pueden ejecutarse en los agentes.

## Ejemplos

- Iniciar Covenant:

  ```bash
  dotnet Covenant.dll
  ```

- Acceder a la interfaz web:

  Abrir `https://localhost:7443` en el navegador.

- Crear un listener y generar un payload para el agente.
