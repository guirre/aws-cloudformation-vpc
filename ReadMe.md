# Cloudformation : VPC

Apprendre comment travailler avec les stack : Aws Cloudformation
Suivre l'article sur : https://www.infoq.com/articles/aws-vpc-cloudformation
Mais pour cela il faut preparer et configurer le compte AWS qui va excecuter aà partir du AWS CLI les commandes de cr&ation de modification 

## Configurer AWS CLI compte 
```
PS C:\outils\AWS\aws-vpc-cloudformation> aws configure
AWS Access Key ID [****************YXYA]: XXXXXXXXXXXXXXXXX
AWS Secret Access Key [****************FjVB]: XXXXXXXXXXXXXXXXXXX
Default region name [eu-west-3]:
Default output format [json]:
```

## Exceutter la commmande de création de VPC avec CloudFormation
```
PS C:\outils\AWS\aws-vpc-cloudformation> aws cloudformation create-stack --stack-name MonReseau --template-body file://MyNetwork.yml
{
    "StackId": "arn:aws:cloudformation:eu-west-3:XXXXXXXXXXXX:stack/MonReseau/d1e01060-0da8-11e9-965f-0eeeeca3615c"
}
```

## Mise a jour du Stack  et suppression de la Stack
```
PS C:\outils\AWS\aws-vpc-cloudformation> aws cloudformation update-stack --stack-name MonReseau --template-body file://MyNetwork.yml
{
    "StackId": "arn:aws:cloudformation:eu-west-3:XXXXXXXXXXX:stack/MonReseau/d1e01060-0da8-11e9-965f-0eeeeca3615c"
}


PS C:\outils\AWS\aws-vpc-cloudformation>
PS C:\outils\AWS\aws-vpc-cloudformation> aws cloudformation delete-stack --stack-name MonReseau
```

### Création d'un Internet GateWay et Attacher cet Internet gateWay à notre VPC

### Création du sous reseau Subnet  (2 Public Subnet et 2 Private Subnet)

### Ajouter une table de routage public et ajout d'une ligne dans la table de Routre

### Création d'une table de routage privée et NAT (Private route table can access web via NAT)

###  Attach the public subnets to public route tables,  and attach the private subnets to private route tables: 


