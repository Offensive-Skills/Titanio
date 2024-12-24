### **Seguridad/PowerView/powerview.md**

# PowerView

## Descripción

`PowerView` es una herramienta de PowerShell diseñada para la enumeración y recopilación de información en entornos de Active Directory. Facilita tareas como la identificación de dominios, usuarios, grupos, computadoras y permisos, siendo útil para profesionales de seguridad y administradores de sistemas en auditorías y pruebas de penetración.

## Uso

PowerView se ejecuta dentro de PowerShell en el contexto de un entorno Windows con Active Directory.

### Cargar PowerView

1. **Descargar PowerView** desde su [repositorio oficial](https://github.com/PowerShellMafia/PowerSploit/tree/master/Recon).
2. **Importar el módulo** en PowerShell:

   ```powershell
   Import-Module .\PowerView.ps1
   ```

### Comandos principales

- `Get-NetDomain`: Enumera información sobre dominios.
- `Get-NetUser`: Recupera información sobre usuarios.
- `Get-NetGroup`: Lista grupos en el dominio.
- `Get-NetComputer`: Obtiene información sobre computadoras.
- `Find-LocalAdminAccess`: Busca cuentas con acceso administrativo local.
- `Invoke-UserHunter`: Identifica usuarios con permisos elevados.
- `Get-NetSession`: Muestra sesiones de red activas.
- `Get-NetShare`: Enumera recursos compartidos en la red.

## Ejemplos

- **Enumerar todos los usuarios en el dominio**:
  
  ```powershell
  Get-NetUser
  ```

- **Listar todos los grupos en el dominio**:
  
  ```powershell
  Get-NetGroup
  ```

- **Obtener información detallada de una computadora específica**:
  
  ```powershell
  Get-NetComputer -ComputerName "Servidor1"
  ```

- **Buscar cuentas con acceso administrativo local**:
  
  ```powershell
  Find-LocalAdminAccess
  ```

- **Enumerar todas las sesiones de red activas**:
  
  ```powershell
  Get-NetSession
  ```

- **Listar todos los recursos compartidos en la red**:
  
  ```powershell
  Get-NetShare
  ```
