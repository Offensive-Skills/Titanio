### **Seguridad/Cifrado/gpg.md**

# gpg

## Descripción

`gpg` (GNU Privacy Guard) es una herramienta para cifrar y firmar datos y comunicaciones. Proporciona criptografía de clave pública para asegurar información, permitiendo cifrar datos y crear firmas digitales.

## Uso

```bash
gpg [opciones] archivos
```

### Opciones principales

- `--gen-key`: Genera un nuevo par de claves.
- `--list-keys`: Lista las claves públicas en el anillo de claves.
- `--list-secret-keys`: Lista las claves privadas.
- `--import`: Importa una clave al anillo de claves.
- `--export`: Exporta una clave pública.
- `--encrypt`: Cifra archivos o mensajes.
- `--decrypt`: Descifra archivos o mensajes.
- `--sign`: Firma digitalmente un archivo.
- `--verify`: Verifica una firma digital.

## Ejemplos

- Generar un nuevo par de claves:

  ```bash
  gpg --gen-key
  ```

- Cifrar un archivo para un destinatario:

  ```bash
  gpg --encrypt --recipient usuario@example.com archivo.txt
  ```

- Descifrar un archivo:

  ```bash
  gpg --decrypt archivo.txt.gpg
  ```

- Firmar un archivo:

  ```bash
  gpg --sign archivo.txt
  ```

- Verificar una firma:

  ```bash
  gpg --verify archivo.txt.gpg
  ```
