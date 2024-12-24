### **Mobile_Security/Drozer/drozer.md**

# Drozer

## Descripción

`Drozer` es una herramienta de seguridad para dispositivos Android que permite a los investigadores de seguridad evaluar la seguridad de aplicaciones Android y detectar vulnerabilidades mediante la interacción con componentes de aplicaciones y el sistema operativo.

## Uso

```bash
drozer console connect
```

### Comandos principales

- `run app.package.list`: Lista las aplicaciones instaladas.
- `run app.package.info -a <package_name>`: Muestra información de una aplicación específica.
- `run app.activity.info -a <package_name>`: Detalla las actividades de una aplicación.
- `run exploit.provider.leak`: Ejecuta un exploit para filtrar datos de proveedores de contenido.

## Ejemplos

- **Listar todas las aplicaciones instaladas:**
  
  ```bash
  drozer> run app.package.list
  ```

- **Obtener información de una aplicación específica:**
  
  ```bash
  drozer> run app.package.info -a com.example.app
  ```

- **Ejecutar un exploit para filtrar datos:**
  
  ```bash
  drozer> run exploit.provider.leak
  ```
