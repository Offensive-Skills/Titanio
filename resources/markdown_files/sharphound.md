### **Análisis de Red/SharpHound/sharphound.md**

# SharpHound

## Descripción

**SharpHound** es el recopilador de datos utilizado por BloodHound. Es una herramienta escrita en .NET que recopila información de Active Directory necesaria para que BloodHound pueda analizarla.

## Uso

```cmd
SharpHound.exe [opciones]
```

### Opciones principales

- `--CollectionMethod`: Especifica el método de recopilación (Default, All, Group, LocalGroup, etc.).
- `--Domain`: Especifica el dominio a analizar.
- `--LDAPUser`: Usuario para autenticación LDAP.
- `--LDAPPass`: Contraseña para autenticación LDAP.
- `--OutputDirectory`: Directorio donde se guardarán los resultados.

## Ejemplos

- Recopilar toda la información:

  ```cmd
  SharpHound.exe --CollectionMethod All
  ```

- Especificar directorio de salida:

  ```cmd
  SharpHound.exe --OutputDirectory "C:\Resultados"
  ```

