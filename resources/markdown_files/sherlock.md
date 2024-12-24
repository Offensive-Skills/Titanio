### **Herramientas de Seguridad/Enumeración/Sherlock.md**

# Sherlock

## Descripción

`Sherlock` es un script en PowerShell que busca vulnerabilidades conocidas de escalada de privilegios locales en sistemas Windows. Compara la versión del sistema operativo con una base de datos de vulnerabilidades para identificar posibles exploits.

## Uso

Ejecutar el script en PowerShell.

```powershell
Import-Module .\Sherlock.ps1
Find-AllVulnerabilities
```

### Cmdlets principales

- `Find-AllVulnerabilities`: Busca todas las vulnerabilidades conocidas.
- `Find-PrivilegeEscalation`: Busca vulnerabilidades específicas para escalada de privilegios.
- `Get-ExploitMitigations`: Muestra mitigaciones y parches instalados.

## Ejemplos

- Ejecutar todas las comprobaciones de vulnerabilidades:

  ```powershell
  Find-AllVulnerabilities
  ```

- Buscar vulnerabilidades específicas:

  ```powershell
  Find-PrivilegeEscalation -Name MS16-032
  ```
