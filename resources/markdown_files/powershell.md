### **Programming_Languages/PowerShell/powershell.md**

# PowerShell

## Descripción

`PowerShell` es un shell de línea de comandos y lenguaje de scripting desarrollado por Microsoft. Está diseñado para la automatización de tareas de administración del sistema y la gestión de configuraciones en entornos Windows, aunque también es compatible con Linux y macOS.

## Uso

```powershell
powershell [opciones] -File script.ps1
```

### Opciones principales

- `-Command`: Ejecuta comandos de PowerShell directamente.
- `-File`: Ejecuta un script de PowerShell.
- `-ExecutionPolicy`: Define la política de ejecución de scripts.
- `-NoProfile`: Inicia PowerShell sin cargar el perfil del usuario.

## Ejemplos

- **Ejecutar un script de PowerShell:**
  
  ```powershell
  powershell -File script.ps1
  ```

- **Ejecutar un comando directamente:**
  
  ```powershell
  powershell -Command "Get-Process"
  ```

- **Iniciar PowerShell sin cargar el perfil:**
  
  ```powershell
  powershell -NoProfile
  ```

- **Establecer la política de ejecución a Bypass:**
  
  ```powershell
  powershell -ExecutionPolicy Bypass -File script.ps1
  ```

