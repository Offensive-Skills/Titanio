### **Virtualización/VBoxManage/vboxmanage.md**

# VBoxManage

## Descripción

`VBoxManage` es la herramienta de línea de comandos para administrar máquinas virtuales en VirtualBox. Permite crear, configurar, iniciar, pausar y gestionar diversos aspectos de las máquinas virtuales, proporcionando un control completo sin necesidad de usar la interfaz gráfica.

## Uso

```bash
VBoxManage comando [opciones]
```

### Comandos principales

- `createvm`: Crea una nueva máquina virtual.
- `modifyvm`: Modifica las configuraciones de una máquina virtual existente.
- `startvm`: Inicia una máquina virtual.
- `controlvm`: Controla una máquina virtual en ejecución (pausar, reiniciar, apagar).
- `list vms`: Lista todas las máquinas virtuales registradas.
- `list runningvms`: Lista las máquinas virtuales en ejecución.
- `clonevm`: Clona una máquina virtual existente.
- `snapshot`: Gestiona snapshots de una máquina virtual.

## Ejemplos

- Crear una nueva máquina virtual:
  
  ```bash
  VBoxManage createvm --name "MiVM" --ostype Ubuntu_64 --register
  ```

- Modificar la cantidad de RAM de una máquina virtual:
  
  ```bash
  VBoxManage modifyvm "MiVM" --memory 2048
  ```

- Iniciar una máquina virtual:
  
  ```bash
  VBoxManage startvm "MiVM" --type headless
  ```

- Listar todas las máquinas virtuales:
  
  ```bash
  VBoxManage list vms
  ```

- Apagar una máquina virtual en ejecución:
  
  ```bash
  VBoxManage controlvm "MiVM" acpipowerbutton
  ```

- Crear un snapshot:
  
  ```bash
  VBoxManage snapshot "MiVM" take "SnapshotInicial"
  ```
