### **Explotación de Active Directory/ASREPRoast.md**

# ASREPRoast

## Descripción

`ASREPRoast` es una técnica de ataque que aprovecha la función de servicio de autenticación de Active Directory para obtener tickets de servicio AS-REP. Estos tickets pueden ser crackeados para revelar contraseñas de cuentas que no requieren autenticación de Kerberos (cuentas sin Kerberos preautenticado).

## Uso

```bash
asreprorast [opciones]
```

### Opciones principales

- `-u`, `--user`: Nombre de usuario objetivo.
- `-d`, `--domain`: Dominio objetivo.
- `--output`: Archivo de salida para los tickets obtenidos.
- `-h`, `--help`: Muestra la ayuda y opciones disponibles.

## Ejemplos

- Extraer tickets AS-REP para un usuario específico:
  
  ```bash
  asreprorast.py -u usuario -d ejemplo.com --output asrep_tickets.kirbi
  ```

- Realizar ASREPRoasting en múltiples usuarios:
  
  ```bash
  asreprorast.py -u usuarios.txt -d ejemplo.com --output asrep_tickets.kirbi
  ```
