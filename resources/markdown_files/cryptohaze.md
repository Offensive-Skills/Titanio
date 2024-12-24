### **Herramientas de Seguridad/Cracking de Contraseñas/cryptohaze.md**

# Cryptohaze

## Descripción

**Cryptohaze** es un conjunto de herramientas de código abierto diseñadas para acelerar el cracking de hashes utilizando GPUs (procesadores gráficos). Incluye aplicaciones como multiforcer y rainbow tables para descifrar hashes comunes como MD5, NTLM y otros.

## Uso

Las herramientas de Cryptohaze se ejecutan desde línea de comandos y aprovechan el procesamiento paralelo de las GPUs para acelerar los ataques.

### Características principales

- **Multiforcer**: Soporta múltiples tipos de hashes y realiza ataques de fuerza bruta.
- **Rainbow Tables**: Genera y utiliza tablas arcoíris para acelerar el cracking.
- **Compatibilidad**: Funciona en sistemas Windows, Linux y macOS con soporte CUDA y OpenCL.

## Ejemplos

- Ejecutar Multiforcer para MD5:

  ```bash
  ./Cryptohaze-Multiforcer -h MD5 -f hashes.txt
  ```

- Utilizar OpenCL en lugar de CUDA:

  ```bash
  ./Cryptohaze-Multiforcer -h NTLM -f hashes.txt --opencl
  ```

- Generar tablas arcoíris:

  ```bash
  ./Cryptohaze-Rainbow-Table-Generator -t NTLM -b 8 -o tabla.rt
  ```



