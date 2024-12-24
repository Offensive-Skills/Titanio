### **Análisis de Red/ldapsearch/ldapsearch.md**

# ldapsearch

## Descripción

`ldapsearch` es una herramienta de línea de comandos que se utiliza para buscar y recuperar información de servidores LDAP (Lightweight Directory Access Protocol). Es útil para consultar y depurar directorios LDAP.

## Uso

```bash
ldapsearch [opciones] [filtro] [atributos]
```

### Opciones principales

- `-x`: Utiliza autenticación simple (no SASL).
- `-H`: Especifica la URL del servidor LDAP.
- `-D`: DN (Distinguished Name) del usuario para autenticación.
- `-W`: Solicita la contraseña de forma interactiva.
- `-w`: Especifica la contraseña en línea (no recomendado).
- `-b`: Base DN desde donde iniciar la búsqueda.

## Ejemplos

- Búsqueda anónima de todos los objetos:

  ```bash
  ldapsearch -x -H ldap://servidor -b "dc=ejemplo,dc=com"
  ```

- Búsqueda con autenticación:

  ```bash
  ldapsearch -x -H ldap://servidor -D "cn=admin,dc=ejemplo,dc=com" -W -b "dc=ejemplo,dc=com"
  ```

- Buscar usuarios específicos:

  ```bash
  ldapsearch -x -H ldap://servidor -b "dc=ejemplo,dc=com" "(uid=usuario1)"
  ```
