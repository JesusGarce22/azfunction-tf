### **Lab de Terraform**
Encontramos la siguiente estructura de carpetas y archivos

```
  example
  main.tf
  variables.tf
```

Para esta practica usamos la funcionalidad de codespaces.

Lo primero que hicimos fue instalar las herramientas necesarias

* [Terraform](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/function_app)
* [Azure-cli](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)

Primero nos autenticamos usando las credenciales de AZURE


Luego usamos el comando **terraform validate** para comprobar que los archivos de configuración de Terraform están bien formados y no contienen errores de sintaxis o lógica.
```
terraform validate
```
Luego usamos **terraform plan** que genera un plan de ejecución que describe los cambios que Terraform realizará en la infraestructura. Es un paso de previsualización que no realiza cambios, pero muestra qué recursos se crearán, modificarán o destruirán.
```
terraform plan
```
Luego, **terraform apply** que aplica el plan de ejecución a la infraestructura real. Este es el paso donde los cambios se implementan, creando, modificando o destruyendo recursos según lo indicado por los archivos de configuración.

```
terraform aplly
```
![](/imgs/WhatsApp%20Image%202024-09-11%20at%209.03.01%20PM.jpeg)

Para eliminar la infraestructura creada, se puede utilizar:

```bash
terraform destroy
```
![](/imgs/WhatsApp%20Image%202024-09-11%20at%209.12.33%20PM.jpeg)

Evidencias

![](/imgs/WhatsApp%20Image%202024-09-11%20at%209.06.09%20PM.jpeg)
![](/imgs/WhatsApp%20Image%202024-09-11%20at%209.07.00%20PM.jpeg)