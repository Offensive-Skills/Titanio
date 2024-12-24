### **Herramientas de Seguridad/Cracking de Contraseñas/hashcat_utils.md**

# hashcat-utils

## Descripción

`hashcat-utils` es un conjunto de pequeñas utilidades diseñadas para complementar las funciones de hashcat. Incluyen herramientas para manipular diccionarios, generar máscaras, combinar reglas y más, facilitando la preparación de datos para ataques de cracking.

## Uso

Las utilidades se ejecutan desde la línea de comandos y cada una tiene su propio conjunto de opciones.

### Herramientas principales

- `cap2hccapx`: Convierte archivos .cap (capturas de paquetes) a .hccapx para ataques WPA/WPA2.
- `combinator`: Combina dos diccionarios, concatenando cada palabra de uno con cada palabra del otro.
- `len`: Filtra palabras de un diccionario por longitud.
- `maskprocessor`: Genera listas de palabras basadas en máscaras definidas.

## Ejemplos

- Convertir un archivo .cap a .hccapx:

  ```bash
  ./cap2hccapx captura.cap salida.hccapx
  ```

- Combinar dos diccionarios:

  ```bash
  ./combinator diccionario1.txt diccionario2.txt > combinado.txt
  ```

- Filtrar palabras de longitud 8 a 12:

  ```bash
  ./len 8 12 < diccionario.txt > filtrado.txt
  ```

- Generar palabras con máscara:

  ```bash
  ./maskprocessor ?u?l?l?l?d?d > palabras.txt
  ```
