### **Version_Control/DVCS_Pillage/dvcs_pillage.md**

# DVCS Pillage

## Descripción

`DVCS Pillage` es una herramienta diseñada para extraer información sensible de sistemas de control de versiones distribuidos (DVCS) como Git, Subversion y Mercurial. Facilita la recopilación de datos expuestos accidentalmente en repositorios públicos o mal configurados.

## Uso

```bash
dvcs_pillage [opciones] <URL_repositorio>
```

### Opciones principales

- `-t, --tokens`: Busca tokens y claves API en el historial del repositorio.
- `-f, --files`: Enumera archivos sensibles presentes en el repositorio.
- `-d, --depth`: Define la profundidad del análisis en el historial.
- `-o, --output archivo`: Guarda los resultados en un archivo especificado.
- `-h, --help`: Muestra la ayuda y las opciones disponibles.

## Ejemplos

- **Escanear un repositorio para encontrar tokens API:**

  ```bash
  dvcs_pillage -t https://github.com/usuario/repo.git
  ```

- **Buscar archivos sensibles y guardar resultados:**

  ```bash
  dvcs_pillage -f -o resultados.txt https://github.com/usuario/repo.git
  ```

- **Analizar con una profundidad específica:**

  ```bash
  dvcs_pillage -d 50 https://github.com/usuario/repo.git
  ```

