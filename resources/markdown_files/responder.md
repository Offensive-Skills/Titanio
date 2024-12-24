### **Network_Security/Responder/responder.md**

# Responder

## Descripción

`Responder` es una herramienta de seguridad de red de código abierto diseñada para capturar y analizar tráfico de red en entornos Windows. Utiliza técnicas de envenenamiento de protocolos como LLMNR, NBT-NS y MDNS para interceptar credenciales y realizar ataques de hombre en el medio (MITM).

## Uso

```bash
responder [opciones]
```

### Opciones principales

- `-I interfaz`: Especifica la interfaz de red a utilizar (por ejemplo, `eth0`, `wlan0`).
- `-A`: Activa todos los ataques de protocolo disponibles.
- `-r`: Habilita el envenenamiento de LLMNR, NBT-NS y MDNS.
- `-w`: Inicia el servidor HTTP para capturar solicitudes.
- `-f`: Fuerza la captura de credenciales incluso si ya existen en la base de datos.
- `-v`: Modo detallado, muestra información adicional durante la ejecución.
- `--disable-ntlmv2`: Desactiva el uso de NTLMv2 para capturar hashes NTLMv1.

## Ejemplos

- **Ejecutar `Responder` en la interfaz `eth0` con todos los ataques habilitados:**

  ```bash
  responder -I eth0 -A
  ```

- **Habilitar envenenamiento de protocolos y servidor HTTP:**

  ```bash
  responder -I wlan0 -r -w
  ```

- **Ejecutar `Responder` en modo detallado:**

  ```bash
  responder -I eth0 -A -v
  ```

- **Capturar credenciales sin utilizar NTLMv2:**

  ```bash
  responder -I eth0 -A --disable-ntlmv2
  ```

- **Forzar la captura de credenciales existentes:**

  ```bash
  responder -I eth0 -A -f
  ```
