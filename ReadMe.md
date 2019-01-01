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
