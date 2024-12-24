### **Seguridad/Cifrado/openssl.md**

# openssl

## Descripción

`openssl` es una poderosa herramienta de línea de comandos para manejar tareas relacionadas con criptografía, incluyendo generación de claves, creación de certificados, cifrado y descifrado de datos, y más. Es parte del proyecto OpenSSL que implementa protocolos y estándares criptográficos.

## Uso

```bash
openssl comando [opciones]
```

### Comandos principales

- `genrsa`: Genera claves privadas RSA.
- `rsa`: Gestiona claves RSA (ver, convertir).
- `req`: Gestiona solicitudes de certificado (CSR).
- `x509`: Gestiona certificados X.509.
- `enc`: Cifra y descifra datos.
- `dgst`: Calcula sumas de verificación y hashes.
- `s_client`: Cliente SSL/TLS para pruebas.

## Ejemplos

- Generar una clave privada RSA de 2048 bits:

  ```bash
  openssl genrsa -out clave.pem 2048
  ```

- Crear una solicitud de certificado (CSR):

  ```bash
  openssl req -new -key clave.pem -out solicitud.csr
  ```

- Cifrar un archivo con AES-256-CBC:

  ```bash
  openssl enc -aes-256-cbc -salt -in archivo.txt -out archivo.enc
  ```

- Descifrar un archivo cifrado:

  ```bash
  openssl enc -d -aes-256-cbc -in archivo.enc -out archivo.txt
  ```

- Ver los detalles de un certificado:

  ```bash
  openssl x509 -in certificado.crt -text -noout
  ```

