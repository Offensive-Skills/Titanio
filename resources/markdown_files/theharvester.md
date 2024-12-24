### **Miscelánea/Recolección de Información/TheHarvester.md**

# TheHarvester

## Descripción

`TheHarvester` es una herramienta de recolección de información utilizada para obtener datos sobre dominios, correos electrónicos, hosts y subdominios. Utiliza fuentes públicas y motores de búsqueda para recopilar información que puede ser útil en fases iniciales de pruebas de penetración.

## Uso

```bash
theharvester [opciones]
```

### Opciones principales

- `-d`, `--domain`: Dominio objetivo para la recolección.
- `-b`, `--source`: Fuente de búsqueda (e.g., google, bing, linkedin).
- `-l`, `--limit`: Número máximo de resultados a obtener.
- `-g`, `--google-hack`: Ejecuta búsquedas avanzadas de Google.
- `-v`, `--verbose`: Modo detallado.
- `-h`, `--help`: Muestra la ayuda y opciones disponibles.

## Ejemplos

- Buscar correos electrónicos en el dominio ejemplo.com usando Google:
  
  ```bash
  theharvester -d ejemplo.com -b google -l 500 -f resultado.html
  ```

- Enumerar subdominios de ejemplo.com usando Bing:
  
  ```bash
  theharvester -d ejemplo.com -b bing -l 300 -f subdominios.html
  ```

- Realizar búsquedas avanzadas de Google:
  
  ```bash
  theharvester -d ejemplo.com -b google-hack -l 100 -f google_hack.html
  ```

- Obtener resultados verbosos de la búsqueda en LinkedIn:
  
  ```bash
  theharvester -d ejemplo.com -b linkedin -l 200 -v -f linkedin_resultados.html
  ```
