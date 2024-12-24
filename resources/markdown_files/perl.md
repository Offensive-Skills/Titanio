### **Programming_Languages/Perl/perl.md**

# Perl

## Descripción

`Perl` es un lenguaje de programación de alto nivel, interpretado y de propósito general. Es conocido por su capacidad de manipulación de texto y es ampliamente utilizado en administración de sistemas, desarrollo web, análisis de datos y scripting.

## Uso

```bash
perl [opciones] script.pl [argumentos]
```

### Opciones principales

- `-e`: Ejecuta código Perl proporcionado como cadena.
- `-c`: Verifica la sintaxis del script sin ejecutarlo.
- `-w`: Habilita los warnings para detectar posibles problemas.
- `-i`: Edita archivos en el lugar.

## Ejemplos

- **Ejecutar un script Perl:**
  
  ```bash
  perl script.pl
  ```

- **Ejecutar código Perl directamente:**
  
  ```bash
  perl -e "print 'Hello, Perl!\n';"
  ```

- **Verificar la sintaxis de un script:**
  
  ```bash
  perl -c script.pl
  ```

- **Editar un archivo en el lugar con backups:**
  
  ```bash
  perl -i.bak -pe 's/old/new/g' archivo.txt
  ```
