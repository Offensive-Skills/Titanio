### **Cloud/Azure_CLI/azure_cli.md**

# Azure CLI

## Descripción

`Azure CLI` es una herramienta de línea de comandos para gestionar recursos de Microsoft Azure. Permite crear, administrar y automatizar servicios de Azure desde la terminal.

## Uso

```bash
az [comando] [subcomando] [opciones]
```

### Comandos principales

- `az login`: Autentica al usuario en Azure.
- `az group create`: Crea un grupo de recursos.
- `az vm list`: Lista las máquinas virtuales.
- `az storage account create`: Crea una cuenta de almacenamiento.

## Ejemplos

- **Iniciar sesión en Azure:**

  ```bash
  az login
  ```

- **Crear un grupo de recursos:**

  ```bash
  az group create --name MiGrupo --location eastus
  ```

- **Listar máquinas virtuales:**

  ```bash
  az vm list --output table
  ```

- **Crear una cuenta de almacenamiento:**

  ```bash
  az storage account create --name micuenta --resource-group MiGrupo --location westus
  ```

