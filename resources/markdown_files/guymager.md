### **Análisis Forense/Guymager/guymager.md**

# Guymager

## Descripción

**Guymager** es una aplicación gráfica para Linux que permite la adquisición forense de medios de almacenamiento. Ofrece una interfaz sencilla y soporte para múltiples formatos de imágenes, facilitando la creación rápida y eficiente de imágenes forenses.

## Uso

Guymager se ejecuta en sistemas Linux y requiere privilegios de administrador para acceder a dispositivos de almacenamiento.

### Características principales

- **Creación de imágenes**: Soporta formatos EWF (E01), AFF y RAW.
- **Velocidad optimizada**: Utiliza múltiples hilos para acelerar la adquisición.
- **Verificación de integridad**: Calcula y verifica hashes MD5 y SHA1 en tiempo real.
- **Registro detallado**: Genera logs con información del proceso de adquisición.

## Ejemplos de uso

- **Crear una imagen de un dispositivo**:

  - Iniciar Guymager con privilegios de administrador.
    ```bash
    sudo guymager
    ```
  - Seleccionar el dispositivo a adquirir.
  - Hacer clic derecho y seleccionar "Acquire Image".
  - Configurar las opciones de imagen y destino.
