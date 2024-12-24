### **Ingeniería Social/Gophish.md**

# Gophish

## Descripción

`Gophish` es una herramienta de phishing de código abierto que facilita la creación y gestión de campañas de phishing. Ofrece una interfaz web intuitiva para diseñar correos electrónicos, páginas de destino y rastrear las respuestas de los usuarios.

## Uso

```bash
gophish
```

### Opciones principales

- `-config`: Especifica el archivo de configuración.
- `-port`: Define el puerto en el que se ejecuta el servidor web.
- `-debug`: Activa el modo de depuración.

## Ejemplos

- Iniciar Gophish con un archivo de configuración específico:

  ```bash
  gophish -config config.json
  ```

- Ejecutar Gophish en modo de depuración:

  ```bash
  gophish -debug
  ```

- Acceder a la interfaz web de Gophish:

  1. Inicia Gophish:

     ```bash
     gophish
     ```

  2. Abre un navegador y navega a `http://localhost:3333`.
  3. Inicia sesión con las credenciales configuradas.
