### **Hacking Web/Inyecciones SQL/BBQSQL.md**

# BBQSQL

## Descripción

`BBQSQL` es una herramienta de inyección SQL ciega que utiliza técnicas de fuerza bruta para extraer datos de bases de datos vulnerables. Está diseñada para entornos donde las respuestas de la aplicación web son limitadas o no contienen información útil para detectar inyecciones.

## Uso

```bash
bbqsql [opciones]
```

### Opciones principales

- `-u URL`: Especifica la URL objetivo para la inyección SQL.
- `-p PARAM`: Define el parámetro vulnerable a probar.
- `--technique TECH`: Selecciona la técnica de inyección (boolean, time, etc.).
- `--threads N`: Define el número de hilos para acelerar la explotación.
- `--dump`: Extrae el contenido de la base de datos.
- `--dbs`: Enumera las bases de datos disponibles.
- `--tables`: Enumera las tablas de una base de datos específica.
- `--columns`: Enumera las columnas de una tabla específica.

## Ejemplos

- Probar una URL para inyección SQL y enumerar las bases de datos:
  
  ```bash
  bbqsql -u "http://example.com/page.php?id=1" -p id --technique boolean --dbs
  ```

- Extraer todas las tablas de una base de datos específica:
  
  ```bash
  bbqsql -u "http://example.com/page.php?id=1" -p id --technique boolean -D nombre_db --tables --dump
  ```

- Extraer columnas específicas de una tabla:
  
  ```bash
  bbqsql -u "http://example.com/page.php?id=1" -p id --technique boolean -D nombre_db -T nombre_tabla --columns columna1,columna2 --dump
  ```

- Usar múltiples hilos para acelerar la explotación:
  
  ```bash
  bbqsql -u "http://example.com/page.php?id=1" -p id --technique boolean --threads 10 --dbs
  ```
