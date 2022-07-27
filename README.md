# Criação de cluster AKS<br />

### Criando cluster com base na documentação e ajustando de acordo com o necessário<br />
### Aqui será para deploy de um wordpress.<br />

## Conteiner Registry: <b>dukercsmcr1</b><br />
## AKS Nome do cluster: wordpress-aks<br />
## Esta guardando o arquivo de estado do terraform em um blob: tfstateactions<br />
## Cria a associação entre o ACR e o AKS (Registry e Cluster)<br />
<br />

## Necessário passar variaveis de acesso ao azure <b>appID</b> e **Password**<br />
### O plan pode ser feito com um arquivo de variaveis ou -var="appId=XPTY..." e -var="password=QWERTY..."<br /><br />
<i>terraform init</i><br />
<i>terraform plan -var-file acesso.tfvars -out aks_plan.tfplan <br />
terraform apply aks_plan.tfplan</i>
