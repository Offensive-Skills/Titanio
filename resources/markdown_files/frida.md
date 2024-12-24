### **Mobile_Security/Frida/frida.md**

# Frida

## Descripción

`Frida` es una herramienta de instrumentación dinámica que permite inyectar scripts en tiempo de ejecución en aplicaciones nativas, móviles y de escritorio. Es utilizada para ingeniería inversa, análisis de seguridad y pruebas de penetración.

## Uso

```bash
frida -U -f <app_package> -l <script.js> --no-pause
```

### Opciones principales

- `-U`: Conecta a un dispositivo USB.
- `-f`: Inicia la aplicación especificada.
- `-l`: Carga un script JavaScript.
- `--no-pause`: No pausa la aplicación después de inyectar el script.

## Ejemplos

- **Inyectar un script en una aplicación Android:**
  
  ```bash
  frida -U -f com.example.app -l script.js --no-pause
  ```

- **Listar todos los procesos activos:**
  
  ```bash
  frida-ps -U
  ```

- **Iniciar una sesión interactiva:**
  
  ```bash
  frida -U -i com.example.app
  ```
