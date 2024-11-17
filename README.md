<!-- BEGIN_TF_DOCS -->
# Curso Arquitetura de Containers na AWS 
## Aula 01 - VPC
> Exemplos de implementação dos exercícios desenvolvidos na aula sobre criação e planejamento de VPC's de alta disponibilidade para arquiteturas de containers
> 
![Arquitetura](/docs/Linuxtips-Containers-AWS-VPC-Uso.drawio.png)

![Planejamento](/docs/Linuxtips-Containers-AWS-VPC-Planejamento.drawio.png)


## Comandos
```sh
terraform init --backend-config=environment/dev/backend.tfvars
terraform apply --auto-approve -var-file=environment/dev/terraform.tfvars
```

## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | 5.64.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_eip.vpc_eip_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip) | resource |
| [aws_eip.vpc_eip_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip) | resource |
| [aws_eip.vpc_eip_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip) | resource |
| [aws_internet_gateway.gw](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/internet_gateway) | resource |
| [aws_nat_gateway.nat_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway) | resource |
| [aws_nat_gateway.nat_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway) | resource |
| [aws_nat_gateway.nat_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway) | resource |
| [aws_route.private_acess_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route) | resource |
| [aws_route.private_acess_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route) | resource |
| [aws_route.private_acess_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route) | resource |
| [aws_route.public_acess](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route) | resource |
| [aws_route_table.private_internet_access_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table.private_internet_access_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table.private_internet_access_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table.public_internet_access](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table_association.private_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.private_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.private_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.public_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.public_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.public_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_ssm_parameter.database_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter) | resource |
| [aws_ssm_parameter.database_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter) | resource |
| [aws_ssm_parameter.database_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter) | resource |
| [aws_ssm_parameter.private_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter) | resource |
| [aws_ssm_parameter.private_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter) | resource |
| [aws_ssm_parameter.private_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter) | resource |
| [aws_ssm_parameter.public_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter) | resource |
| [aws_ssm_parameter.public_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter) | resource |
| [aws_ssm_parameter.public_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter) | resource |
| [aws_ssm_parameter.vpc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ssm_parameter) | resource |
| [aws_subnet.database_subnet_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.database_subnet_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.database_subnet_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.private_subnet_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.private_subnet_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.private_subnet_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.public_subnet_1a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.public_subnet_1b](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.public_subnet_1c](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_vpc.main](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_project_name"></a> [project\_name](#input\_project\_name) | Nome do projeto. Essa variável será um prefixo para os recursos criados dentro deste projeto | `any` | n/a | yes |
| <a name="input_region"></a> [region](#input\_region) | n/a | `any` | "Região da AWS onde os recursos serão criados" | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_ssm_subnet_database_1a"></a> [ssm\_subnet\_database\_1a](#output\_ssm\_subnet\_database\_1a) | ID da subnet de bancos de dados na zona de disponibilidade 1a. Este ID é recuperado do AWS Systems Manager Parameter Store e usado para o provisionamento de instâncias de banco de dados nesta zona específica. |
| <a name="output_ssm_subnet_database_1b"></a> [ssm\_subnet\_database\_1b](#output\_ssm\_subnet\_database\_1b) | ID da subnet de bancos de dados na zona de disponibilidade 1b. Obtido do AWS Systems Manager Parameter Store, é essencial para a alocação de instâncias de banco de dados que precisam ser isoladas nesta zona. |
| <a name="output_ssm_subnet_database_1c"></a> [ssm\_subnet\_database\_1c](#output\_ssm\_subnet\_database\_1c) | ID da subnet de bancos de dados na zona de disponibilidade 1c, proveniente do AWS Systems Manager Parameter Store. Utilizado no provisionamento de instâncias de banco de dados que requerem isolamento nesta zona. |
| <a name="output_ssm_subnet_private_1a"></a> [ssm\_subnet\_private\_1a](#output\_ssm\_subnet\_private\_1a) | ID da subnet privada na zona de disponibilidade 1a. Valor armazenado no AWS Systems Manager Parameter Store, utilizado para provisionar recursos em uma subnet privada específica. |
| <a name="output_ssm_subnet_private_1b"></a> [ssm\_subnet\_private\_1b](#output\_ssm\_subnet\_private\_1b) | ID da subnet privada na zona de disponibilidade 1b. Armazenado no AWS Systems Manager Parameter Store, usado para alocação de recursos que requerem isolamento dentro desta zona de disponibilidade. |
| <a name="output_ssm_subnet_private_1c"></a> [ssm\_subnet\_private\_1c](#output\_ssm\_subnet\_private\_1c) | ID da subnet privada na zona de disponibilidade 1c. Guardado no AWS Systems Manager Parameter Store, é crucial para a criação de recursos que precisam ser isolados nesta zona específica. |
| <a name="output_ssm_subnet_public_1a"></a> [ssm\_subnet\_public\_1a](#output\_ssm\_subnet\_public\_1a) | ID da subnet pública na zona de disponibilidade 1a. Este ID, proveniente do AWS Systems Manager Parameter Store, é utilizado para provisionar recursos acessíveis publicamente nesta zona. |
| <a name="output_ssm_subnet_public_1b"></a> [ssm\_subnet\_public\_1b](#output\_ssm\_subnet\_public\_1b) | ID da subnet pública na zona de disponibilidade 1b. Disponível via AWS Systems Manager Parameter Store, permite a implementação de recursos com acesso público nesta zona específica. |
| <a name="output_ssm_subnet_public_1c"></a> [ssm\_subnet\_public\_1c](#output\_ssm\_subnet\_public\_1c) | ID da subnet pública na zona de disponibilidade 1c, armazenado no AWS Systems Manager Parameter Store. Usado para configurar recursos que necessitam de acesso público nesta zona. |
| <a name="output_ssm_vpc_id"></a> [ssm\_vpc\_id](#output\_ssm\_vpc\_id) | ID do VPC armazenado no AWS Systems Manager Parameter Store. Este ID é usado para identificar o VPC onde os recursos serão provisionados. |



## Tipos de Subnet:
**Pública:** possui uma rota direta para um internet gateway. Recursos em uma subnet
pública pode acessar a internet. E podem ser acessados, desde que possuam ip
público.

Internet Gateway: é o componente que premit comunicação entre a VPC e a internet.
fornece um destino nas tabelas de rotas da VPC para tráfego roteável pela Internet.
Para a comunicação usando o IPv4, o gateway da Internet também executa a 
conversão de endereços de rede (NAT).
Para tornar a sub-rede pública, adicione uma rota à tabela de rotas da sua 
sub-rede que direcione o tráfego vinculado à Internet para o Internet Gateway.

Se a VPC não tem um Internet Gateway, os recursos da VPC não podem ser acessados
da internet.( A não ser que o tráfego flua via Corporate Network e VPN/Direct 
Connect )

VPC >> Public Network >> Internet Gateway >> Route Table

**Privada:** não tem uma rota direta para um internet gateway. Necessita de um 
dispositivo NAT para acessar a internet.



<!-- END_TF_DOCS -->


