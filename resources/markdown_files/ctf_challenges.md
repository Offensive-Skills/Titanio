### **CTF/CTF_Challenges/ctf_challenges.md**

# CTF Challenges

## Descripción

`CTF Challenges` son conjuntos de problemas diseñados para competiciones de Capture The Flag (CTF). Cubren diversas áreas como criptografía, explotación, ingeniería inversa y análisis forense, desafiando las habilidades de los participantes en seguridad informática.

## Uso

Las challenges pueden ser accedidas a través de plataformas CTF o directamente mediante archivos proporcionados en competiciones locales.

### Tipos comunes de challenges

- **Criptografía:** Resolver cifrados y descifrar mensajes secretos.
- **Explotación:** Encontrar y aprovechar vulnerabilidades en aplicaciones.
- **Ingeniería Inversa:** Analizar binarios para entender su funcionamiento.
- **Forense:** Recuperar información oculta en archivos o sistemas.

## Ejemplos

- **Criptografía: Descifrar un mensaje cifrado con ROT13.**

  ```bash
  echo "Uryyb Jbeyq!" | tr 'A-Za-z' 'N-ZA-Mn-za-m'
  # Salida: Hello World!
  ```

- **Explotación: Encontrar un buffer overflow en una aplicación vulnerable.**

  ```c
  // Código vulnerable en C
  char buffer[10];
  gets(buffer); // Uso inseguro de gets
  ```

- **Ingeniería Inversa: Analizar un binario con Ghidra para encontrar la clave.**

  ```bash
  ghidraRun
  # Importar el binario y buscar la función de verificación de clave.
  ```

- **Forense: Recuperar datos borrados de un archivo usando `foremost`.**

  ```bash
  foremost -i imagen_disco.dd -o recuperados
  ```




