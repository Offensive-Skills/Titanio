# Introducción

![image](./resources/imagen/titanio.png)

Herramienta de **linea de comandos** para la búsqueda de herramientas **(>300)**, tanto **basicos de linux** como una **gran repertorio de herramientas de ciberseguridad.**


# Instalación

Para la intalación de esta herramienta debemos descargarnos las siguientes librerías con **pip3**

> Es requisito obligatorio contar con python3 y pip3 instalado en el sistema.

```bash
pip3 install rich InquirerPy --break-system-packages
```

Una vez instalado, ejecutamos lo siguiente:

```bash
./titanio --update
```

- Crea las carpetas y almacena los fichero de configuración en **/etc/titanio/ y /usr/share/titanio/**.
- Almacena el script en **/usr/local/bin**

> Una vez ejecutado podremos utilizar **titanio** desde cualquier ubicación del sistema. Si queremos actualizar la herramienta para obtener las nuevas herramientas que se añadan, debemos de ejecutar el mismo comando:

```bash
./titanio --update
```

# Guía de uso

## Ejecuión básica

Ejecución normal, usar los menus para buscar herramientas:

```d
titanio
?  Selecciona una opción: 
❯ Básico
  Hacking Web
  Esteganografía
  Criptografía
  Escalada de Privilegios
  Herramientas Auxiliares
  Forense
  Directorio Activo
  Miscelánea
  Hacking Wi-Fi
  Ingeniería Inversa
  Explotación de Redes
  Sistemas de Control de Versiones
  Seguridad en la Nube
  Contenedores y Virtualización
  Móvil
  Automatización y Scripting
  ---------------
  Volver
  Salir
```

## Bśuqueda de herrmientas

```bash
./titanio <tool_name>
```


Realiza una búsqueda en el sistema con el objetivo de mostrar todas las herramientas que alguna parte de su nombre coincida con la **cadena** que ha introduce el usuario.

Ejemplo:

```d
titanio <tool_name>
? Resultados para 'tr': 
❯  > tr
   > traceroute
   > strings
   > XSStrike
   > SSLstrip
   > Cobalt Strike
   > ltrace
   > strace
  ---------------
  Salir
```

## Búsqueda profunda

Realiza una búsqueda en todos los ficheros para mostrar aquellos en los que el texo que has introducido esta en el contenido del fichero:

```d
titanio --deep_search 'Man-in-the-Middle'
? Resultados para búsqueda profunda 'Man-in-the-Middle': 
❯  > Ettercap
   > SSLstrip
   > MITMf
  ---------------
  Salir
```


---
# License 
Titanio © 2024 by Offensive Skills is licensed under Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International

You can read more about the License in the [`LICENSE` documentation](./LICENSE.md)
