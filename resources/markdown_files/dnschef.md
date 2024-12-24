### **Network_Security/DNSChef/dnschef.md**

# DNSChef

## Descripción

`DNSChef` es una herramienta de phishing DNS de código abierto que permite simular un servidor DNS malicioso. Es utilizada para redirigir las solicitudes DNS de un objetivo hacia direcciones IP controladas por el atacante, facilitando ataques de hombre en el medio (MITM) y la captura de datos sensibles.

## Uso

```bash
dnschef [opciones]
```

### Opciones principales

- `--fakeip IP`: Especifica la dirección IP falsa a la que se redirigirán las solicitudes DNS.
- `--interface interfaz`: Define la interfaz de red en la que `DNSChef` escuchará (por ejemplo, `eth0`, `wlan0`).
- `--fakedomains dominio1,dominio2`: Lista de dominios que serán falsificados.
- `--logfile archivo_log`: Guarda los registros de actividad en el archivo especificado.
- `--stop-after N`: Detiene `DNSChef` después de procesar N solicitudes.
- `--disable-logging`: Desactiva el registro de actividades.

## Ejemplos

- **Redirigir todas las solicitudes DNS a una IP específica en la interfaz `eth0`:**

  ```bash
  dnschef --fakeip 192.168.1.100 --interface eth0
  ```

- **Falsificar únicamente los dominios `example.com` y `test.com`:**

  ```bash
  dnschef --fakeip 10.0.0.5 --fakedomains example.com,test.com --interface wlan0
  ```

- **Guardar los registros de actividad en un archivo:**

  ```bash
  dnschef --fakeip 192.168.1.50 --interface eth0 --logfile dns_logs.txt
  ```

- **Detener `DNSChef` después de procesar 100 solicitudes:**

  ```bash
  dnschef --fakeip 192.168.1.50 --interface eth0 --stop-after 100
  ```

- **Ejecutar `DNSChef` sin registrar actividades:**

  ```bash
  dnschef --fakeip 192.168.1.50 --interface eth0 --disable-logging
  ```

