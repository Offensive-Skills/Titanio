### **Hacking Web/Inyecciones SQL/Havij.md**

# Havij

## Descripción

`Havij` es una herramienta automatizada para realizar inyecciones SQL que facilita la explotación de vulnerabilidades en aplicaciones web. Ofrece una interfaz gráfica de usuario amigable y capacidades avanzadas para extraer datos y obtener acceso no autorizado a bases de datos.

## Uso

```bash
havij [opciones]
```

### Opciones principales

- `--url`: Especifica la URL objetivo para la inyección SQL.
- `--method`: Define el método de solicitud HTTP (GET o POST).
- `--data`: Envía datos POST con la solicitud.
- `--db`: Selecciona la base de datos a explotar.
- `--table`: Selecciona la tabla a explotar.
- `--column`: Selecciona las columnas específicas para extraer.
- `--dump`: Extrae el contenido de la base de datos.
- `--scan`: Escanea y detecta vulnerabilidades de inyección SQL.
- `--verbose`: Muestra información detallada durante la ejecución.

## Ejemplos

- Escanear una URL en busca de vulnerabilidades de inyección SQL:
  
  ```bash
  havij --url "http://example.com/page.php?id=1" --scan
  ```

- Extraer todas las tablas de una base de datos específica:
  
  ```bash
  havij --url "http://example.com/page.php?id=1" --db nombre_db --table --dump
  ```

- Extraer columnas específicas de una tabla:
  
  ```bash
  havij --url "http://example.com/page.php?id=1" --db nombre_db --table nombre_tabla --column columna1,columna2 --dump
  ```

- Usar datos POST en la solicitud:
  
  ```bash
  havij --url "http://example.com/login.php" --method POST --data "username=admin&password=admin" --scan
  ```
