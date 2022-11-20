# 02 - Instalación y puesta en marcha
Creación de cuenta en GCP

La plataforma de elección para este curso va a ser Google Cloud Platform (GCP). Sin embargo, se trata de una herramienta que homogeniza
la creación de IaC para cualquier proveedor de servicios, por lo que no es complicado adaptar esto a otras plataformas.



## Instalar Terraform

En primer lugar vamos a empezar con la instalación, vamos a usar la ultima versión estable de Terraform en el momento de crear este curso,
la v1.3.5.


En caso de que uses Mac recomiendo instalarlo a traves de homebrew:

```
brew tap hashicorp/tap (repositorio de hashicorp con todos los paquetes que necesitamos)
brew install hashicorp/tap/terraform
```


Para Windows lo más straightforward es su instalación a traves de chocolatey:
```
choco install terraform
```


La guia de instalación para SOs alternativos como Debian o Ubuntu se encuentra en el siguiente enlace: https://learn.hashicorp.com/tutorials/terraform/install-cli



https://blog.gruntwork.io/why-we-use-terraform-and-not-chef-puppet-ansible-saltstack-or-cloudformation-7989dad2865c




## Comprueba que todo funciona correctamente

Una vez instalado es momento de comprobar que todo funciona correctamente y que tenemos la versión deseada.
`terraform -help`
`terraform -version`

1) `terraform init`
2) `terraform plan`
3) `terraform apply`


## Estructura de un proyecto y modulos

Aqui se debe explicar cual es la estructura recomendada para los proyectos de forma muy sesgada pero dejando claro
que todo es discutible y que considero que es mejor partir de una base bien definida para ponerla en duda más tarde.
De esta forma se deja mucho menos espacio para la ambigüedad.