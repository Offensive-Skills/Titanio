### **Debugging/OllyDbg/ollydbg.md**

# OllyDbg

## Descripción

`OllyDbg` es un depurador de código binario para sistemas Windows, enfocado en la ingeniería inversa y el análisis de malware. Ofrece una interfaz gráfica de usuario que facilita el desensamblado, la depuración y la modificación de programas binarios en tiempo real.

## Uso

`OllyDbg` se ejecuta en entornos Windows con una interfaz gráfica intuitiva.

1. **Iniciar OllyDbg:**
   - Ejecuta el archivo `OllyDbg.exe`.

2. **Cargar un Ejecutable:**
   - Haz clic en "File" > "Open" y selecciona el archivo binario a depurar.

3. **Iniciar la Depuración:**
   - Presiona "F9" para iniciar la ejecución del programa en modo depuración.

4. **Navegar por el Código:**
   - Utiliza el panel de desensamblado para examinar las instrucciones.
   - Coloca puntos de interrupción haciendo clic en la margen izquierda.

5. **Analizar Variables y Memoria:**
   - Observa los registros y la memoria en tiempo real durante la ejecución.

## Características principales

- Desensamblado en tiempo real y análisis de código.
- Soporte para puntos de interrupción y seguimiento de ejecución.
- Visualización de llamadas a funciones y flujo de control.
- Plugins para ampliar funcionalidades.

## Ejemplos

- **Establecer un punto de interrupción:**
  - Haz clic en la margen izquierda junto a la instrucción donde deseas detener la ejecución.

- **Ver los registros:**
  - Observa el panel de "Registers" para ver los valores actuales de los registros de la CPU.

- **Modificar una instrucción en tiempo real:**
  - Haz clic derecho en una instrucción y selecciona "Assemble" para cambiarla.

- **Seguir el flujo de ejecución:**
  - Usa "Step Into" (F7) o "Step Over" (F8) para avanzar línea por línea.
