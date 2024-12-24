### **Herramientas de Seguridad/Cracking de Contraseñas/john.md**

# john

## Descripción

`john`, también conocido como John the Ripper, es una herramienta de seguridad y auditoría de contraseñas utilizada para detectar contraseñas débiles en sistemas operativos y aplicaciones. Permite realizar ataques de fuerza bruta y basados en diccionario para descifrar contraseñas cifradas.

## Uso

```bash
john [opciones] archivo_hash
```

### Opciones principales

- `--wordlist=archivo`: Especifica un archivo de diccionario para ataques basados en palabras.
- `--rules`: Aplica reglas al diccionario para generar variaciones de palabras.
- `--incremental`: Realiza un ataque de fuerza bruta incremental.
- `--show`: Muestra las contraseñas descifradas.
- `--format=formato`: Especifica el formato de hash (ej. raw-md5, sha256crypt).
- `--session=nombre`: Guarda o restaura una sesión de cracking.

## Ejemplos

- Realizar un ataque basado en diccionario:

  ```bash
  john --wordlist=rockyou.txt hashes.txt
  ```

- Realizar un ataque de fuerza bruta incremental:

  ```bash
  john --incremental hashes.txt
  ```

- Mostrar contraseñas descifradas:

  ```bash
  john --show hashes.txt
  ```

- Especificar el formato de hash:

  ```bash
  john --format=raw-md5 hashes.txt
  ```

