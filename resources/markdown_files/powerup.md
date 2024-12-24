### **Herramientas de Seguridad/Enumeración/PowerUp.md**

# PowerUp

## Descripción

`PowerUp` es un script en PowerShell diseñado para ayudar en la escalada de privilegios en sistemas Windows. Automatiza la búsqueda de configuraciones inseguras y vulnerabilidades que podrían permitir a un usuario aumentar sus privilegios.

## Uso

Ejecutar el script en PowerShell.

```powershell
Import-Module .\PowerUp.ps1
Invoke-AllChecks
```

### Cmdlets principales

- `Invoke-AllChecks`: Ejecuta todas las comprobaciones disponibles.
- `Get-ServiceUnquoted`: Busca servicios con rutas sin comillas.
- `Get-RegistryAutoLogon`: Busca credenciales almacenadas en el registro.
- `Get-UnattendedInstallFiles`: Busca archivos de instalación desatendida con credenciales.

## Ejemplos

- Ejecutar todas las comprobaciones:

  ```powershell
  Invoke-AllChecks
  ```

- Buscar servicios con rutas sin comillas:

  ```powershell
  Get-ServiceUnquoted
  ```

- Buscar credenciales en archivos de instalación:

  ```powershell
  Get-UnattendedInstallFiles
  ```

