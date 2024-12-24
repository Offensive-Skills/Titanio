### **Cloud/AWS_CLI/aws_cli.md**

# AWS CLI

## Descripción

`AWS CLI` es una herramienta de línea de comandos que permite gestionar servicios de Amazon Web Services (AWS). Facilita la automatización de tareas y la administración de recursos AWS directamente desde la terminal.

## Uso

```bash
aws [comando] [subcomando] [opciones]
```

### Comandos principales

- `aws configure`: Configura las credenciales y la región por defecto.
- `aws s3 ls`: Lista los buckets de S3.
- `aws ec2 describe-instances`: Muestra información de las instancias EC2.
- `aws lambda invoke`: Invoca una función Lambda.

## Ejemplos

- **Configurar AWS CLI:**

  ```bash
  aws configure
  ```

- **Listar buckets de S3:**

  ```bash
  aws s3 ls
  ```

- **Describir instancias EC2:**

  ```bash
  aws ec2 describe-instances
  ```

- **Invocar una función Lambda:**

  ```bash
  aws lambda invoke --function-name miFuncion output.txt
  ```
