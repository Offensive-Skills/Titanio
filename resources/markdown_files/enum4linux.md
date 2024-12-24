### **Herramientas de Seguridad/Enumeración/enum4linux.md**

# enum4linux

## Descripción

`enum4linux` es una herramienta para enumerar información de sistemas Windows y Samba. Permite obtener usuarios, grupos, recursos compartidos y más, utilizando diversas técnicas.

## Uso

```bash
enum4linux [opciones] host
```

### Opciones principales

- `-U`: Enumera usuarios.
- `-S`: Enumera recursos compartidos.
- `-G`: Enumera grupos.
- `-P`: Enumera políticas de contraseñas.
- `-a`: Ejecuta todas las enumeraciones anteriores.
- `-u`: Especifica el nombre de usuario.
- `-p`: Especifica la contraseña.

## Ejemplos

- Ejecutar una enumeración completa:

  ```bash
  enum4linux -a ejemplo.com
  ```

- Enumerar usuarios:

  ```bash
  enum4linux -U ejemplo.com
  ```

- Especificar credenciales:

  ```bash
  enum4linux -u usuario -p contraseña ejemplo.com
  ```
