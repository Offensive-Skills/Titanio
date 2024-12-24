### **Cloud/CloudBrute/cloudbrute.md**

# CloudBrute

## Descripción

`CloudBrute` es una herramienta de fuerza bruta diseñada para atacar servicios en la nube, como AWS, Azure y GCP. Automatiza el proceso de descubrimiento de credenciales débiles y configuraciones inseguras en entornos de nube.

## Uso

```bash
cloudbrute [opciones] <servicio>
```

### Opciones principales

- `-u, --username usuario`: Define el nombre de usuario a atacar.
- `-p, --password archivo`: Especifica un archivo de diccionario de contraseñas.
- `-t, --threads N`: Establece el número de hilos concurrentes.
- `-s, --service servicio`: Selecciona el servicio en la nube (aws, azure, gcp).
- `-o, --output archivo`: Guarda los resultados en un archivo.

## Ejemplos

- **Realizar un ataque de fuerza bruta en AWS:**

  ```bash
  cloudbrute -u admin -p diccionario.txt -s aws -o resultados_aws.txt
  ```

- **Ataque concurrente en Azure con múltiples hilos:**

  ```bash
  cloudbrute -u user -p passwords.txt -s azure -t 10 -o resultados_azure.txt
  ```

