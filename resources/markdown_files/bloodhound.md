### **Análisis de Red/BloodHound/bloodhound.md**

# BloodHound

## Descripción

**BloodHound** es una herramienta que utiliza grafos para mostrar y analizar las relaciones dentro de un dominio de Active Directory. Permite identificar caminos para escalar privilegios y obtener control del dominio.

## Uso

BloodHound consta de una aplicación cliente y utiliza recopiladores como `SharpHound` para obtener datos.

### Características principales

- **Visualización de grafos**: Muestra relaciones entre usuarios, grupos, permisos y objetos.
- **Análisis de rutas**: Identifica posibles caminos de ataque.
- **Integración con Neo4j**: Utiliza la base de datos de grafos Neo4j.

## Ejemplos de uso

- **Recopilar datos con SharpHound**:

  ```cmd
  SharpHound.exe --CollectionMethod All
  ```

- **Importar datos en BloodHound**:

  - Iniciar Neo4j y BloodHound.
  - Iniciar sesión en BloodHound.
  - Importar los archivos `.zip` generados por SharpHound.
