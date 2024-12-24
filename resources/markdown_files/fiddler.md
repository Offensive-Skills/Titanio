### **Análisis de Tráfico Web/Fiddler.md**

# Fiddler

## Descripción

`Fiddler` es un proxy de depuración web que captura y analiza el tráfico HTTP y HTTPS entre el navegador y el servidor. Es ampliamente utilizado para la depuración de aplicaciones web, permitiendo la inspección y modificación de solicitudes y respuestas.

## Uso

```bash
fiddler [opciones]
```

### Opciones principales

- `-listen`: Inicia Fiddler como un proxy escuchando en un puerto específico.
- `-cert`: Instala el certificado raíz de Fiddler para interceptar tráfico HTTPS.
- `-log`: Define un archivo de registro para guardar las sesiones capturadas.
- `-clearcache`: Limpia la caché de Fiddler al iniciar.
- `-exitafter`: Sale automáticamente después de capturar un número especificado de sesiones.

## Ejemplos

- Iniciar Fiddler y escuchar en el puerto 8888:

  ```bash
  fiddler -listen 8888
  ```

- Instalar el certificado raíz para interceptar tráfico HTTPS:

  ```bash
  fiddler -cert
  ```

- Guardar las sesiones capturadas en un archivo de registro:

  ```bash
  fiddler -log sesiones.log
  ```

- Iniciar Fiddler y limpiar la caché:

  ```bash
  fiddler -clearcache
  ```
