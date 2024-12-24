### **Programming_Languages/Ruby/ruby.md**

# Ruby

## Descripción

`Ruby` es un lenguaje de programación interpretado, de alto nivel y orientado a objetos. Es conocido por su sintaxis limpia y legible, y es ampliamente utilizado en desarrollo web (especialmente con Ruby on Rails), automatización y scripting.

## Uso

```bash
ruby [opciones] script.rb [argumentos]
```

### Opciones principales

- `-e`: Ejecuta código Ruby proporcionado como cadena.
- `-c`: Verifica la sintaxis del script sin ejecutarlo.
- `-w`: Habilita los warnings para detectar posibles problemas.
- `-I`: Añade directorios a la ruta de carga.

## Ejemplos

- **Ejecutar un script Ruby:**
  
  ```bash
  ruby script.rb
  ```

- **Ejecutar código Ruby directamente:**
  
  ```bash
  ruby -e "puts 'Hello, Ruby!'"
  ```

- **Verificar la sintaxis de un script:**
  
  ```bash
  ruby -c script.rb
  ```

- **Añadir un directorio a la ruta de carga:**
  
  ```bash
  ruby -I ./lib script.rb
  ```
