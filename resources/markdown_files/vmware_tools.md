### **Virtualización/VMwareTools/vmwaretools.md**

# VMware Tools

## Descripción

`VMware Tools` es un conjunto de utilidades que mejora el rendimiento y la gestión de máquinas virtuales ejecutadas en entornos VMware. Proporciona funcionalidades como sincronización de tiempo, mejor integración del ratón, carpetas compartidas y gráficos mejorados, facilitando la interacción entre el sistema operativo invitado y el host.

## Uso

### Instalación en una máquina virtual

1. **Iniciar la máquina virtual** en VMware Workstation, VMware Player o VMware ESXi.
2. **Insertar las herramientas de VMware**:
   
   - En el menú de VMware, selecciona `VM` > `Install VMware Tools` o `Reinstall VMware Tools`.
3. **Montar el CD de VMware Tools** en el sistema operativo invitado:
   
   - En Linux:
     
     ```bash
     mount /dev/cdrom /mnt
     ```
   
   - En Windows, se abrirá automáticamente una ventana de instalación.

4. **Ejecutar el instalador**:
   
   - En Linux:
     
     ```bash
     tar -zxvf /mnt/VMwareTools-*.tar.gz -C /tmp/
     cd /tmp/vmware-tools-distrib/
     sudo ./vmware-install.pl
     ```
   
   - En Windows, sigue las instrucciones del asistente de instalación.

5. **Finalizar la instalación** y reiniciar la máquina virtual si es necesario.

### Uso de VMware Tools

- **Sincronización de tiempo**:
  
  Mantiene el reloj del sistema invitado sincronizado con el host.

- **Carpetas compartidas**:
  
  Accede a carpetas del host desde el sistema invitado.

- **Integración del ratón**:
  
  Permite mover el ratón entre el host y el invitado sin problemas.

- **Mejoras gráficas**:
  
  Soporte para resoluciones de pantalla dinámicas y mejor rendimiento gráfico.

## Ejemplos

- **Actualizar VMware Tools en Linux**:
  
  ```bash
  sudo /usr/bin/vmware-toolbox-cmd upgrade install
  ```

- **Montar una carpeta compartida**:
  
  En el host, define una carpeta compartida. En Linux, monta la carpeta con:
  
  ```bash
  sudo mount -t fuse.vmhgfs-fuse .host:/carpeta_compartida /mnt/carpeta_compartida -o allow_other
  ```

- **Verificar el estado de VMware Tools**:
  
  ```bash
  systemctl status vmtoolsd
  ```
