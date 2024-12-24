### **Hacking Web/Directorios/dirbuster.md**

# DirBuster

## Descripción

`DirBuster` es una herramienta de fuerza bruta para la detección de directorios y archivos ocultos en servidores web. Utiliza listas de palabras predefinidas para intentar acceder a rutas potencialmente sensibles, ayudando a identificar puntos de entrada no documentados en aplicaciones web.

## Uso

DirBuster es una aplicación gráfica basada en Java. Se puede ejecutar desde la línea de comandos o a través de su interfaz gráfica.

```bash
dirbuster [opciones]
```

### Opciones principales

- `-u URL`: Especifica la URL objetivo.
- `-w WORDLIST`: Define la lista de palabras a usar para el escaneo.
- `-t THREADS`: Establece el número de hilos para el escaneo.
- `-x EXTENSIONS`: Añade extensiones de archivo a probar.
- `-r`: Usa rutas recursivas durante el escaneo.
- `-o OUTPUT`: Define el archivo de salida para los resultados.

## Ejemplos

- Ejecutar DirBuster con una lista de palabras específica:
  
  ```bash
  dirbuster -u http://ejemplo.com -w /ruta/a/wordlist.txt
  ```

- Añadir extensiones de archivo para probar:
  
  ```bash
  dirbuster -u http://ejemplo.com -w /ruta/a/wordlist.txt -x .php,.html,.txt
  ```

- Aumentar el número de hilos para un escaneo más rápido:
  
  ```bash
  dirbuster -u http://ejemplo.com -w /ruta/a/wordlist.txt -t 50
  ```

- Guardar los resultados en un archivo:
  
  ```bash
  dirbuster -u http://ejemplo.com -w /ruta/a/wordlist.txt -o resultados.txt
  ```
