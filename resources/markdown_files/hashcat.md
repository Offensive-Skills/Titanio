### **Herramientas de Seguridad/Cracking de Contraseñas/hashcat.md**

# hashcat

## Descripción

`hashcat` es una avanzada herramienta de recuperación de contraseñas que utiliza el poder de procesamiento de la CPU y GPU para descifrar hashes de contraseñas. Es ampliamente utilizada en auditorías de seguridad para probar la fortaleza de contraseñas cifradas.

## Uso

```bash
hashcat [opciones] archivo_hash
```

### Opciones principales

- `-m`: Especifica el tipo de hash (ej. 0 para MD5, 1000 para NTLM).
- `-a`: Define el modo de ataque (0 para diccionario, 3 para máscara).
- `-o`: Especifica el archivo de salida para las contraseñas descifradas.
- `--username`: Ignora los nombres de usuario en el archivo de hash.
- `-w`: Establece el nivel de trabajo (0 a 4) para controlar la carga en la GPU.
- `--session`: Nombra una sesión para pausar y reanudar ataques.

## Ejemplos

- Ataque de diccionario usando un archivo de wordlist:

  ```bash
  hashcat -m 0 -a 0 hashes.txt rockyou.txt
  ```

- Ataque de fuerza bruta con una máscara:

  ```bash
  hashcat -m 1000 -a 3 hashes.txt ?a?a?a?a
  ```

- Reanudar una sesión pausada:

  ```bash
  hashcat --session=miSesion --restore
  ```

- Especificar un archivo de salida:

  ```bash
  hashcat -m 0 -a 0 hashes.txt rockyou.txt -o cracked.txt
  ```
