### **Reverse_Engineering/DotPeek/dotpeek.md**

# dotPeek

## Descripción

`dotPeek` es una herramienta de decompilación gratuita desarrollada por JetBrains que permite descompilar ensamblados .NET a código fuente C#. Es útil para desarrolladores y analistas de seguridad que buscan comprender el funcionamiento interno de aplicaciones .NET sin tener acceso al código fuente original.

## Uso

`dotPeek` ofrece una interfaz gráfica de usuario fácil de usar.

1. **Iniciar dotPeek:**
   - Ejecuta el archivo `dotPeek.exe`.

2. **Abrir un Ensamblado:**
   - Haz clic en "File" > "Open" y selecciona el archivo DLL o EXE de .NET que deseas descompilar.

3. **Explorar el Código Fuente:**
   - Navega por el ensamblado en el panel de la izquierda para ver el código C# descompilado en el panel derecho.

4. **Exportar el Código Fuente:**
   - Selecciona el ensamblado y haz clic en "Export to Project" para generar un proyecto de Visual Studio con el código descompilado.

## Características principales

- Descompilación precisa de ensamblados .NET a C#.
- Navegación sencilla a través de namespaces, clases y métodos.
- Integración con otros productos de JetBrains.
- Exportación de código fuente a proyectos de Visual Studio.

## Ejemplos

- **Descompilar una biblioteca .NET:**
  - Abre `mi_biblioteca.dll` en dotPeek para ver todas las clases y métodos en código C#.

- **Exportar un ensamblado a un proyecto de Visual Studio:**
  - Selecciona `app.exe` y usa "Export to Project" para generar un proyecto completo con el código descompilado.

- **Buscar una clase específica:**
  - Utiliza la barra de búsqueda para encontrar `UsuarioService` y examina su implementación.
