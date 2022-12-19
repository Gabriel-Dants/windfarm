# Projeto - Windfarm

> Projeto de Estudo para utilização das ferramentas AWS: Kinesis, S3, Crawlers, Glue, Jobs e Athena.

## Objetivo: 

O presente projeto tem como objetivo simular um sistema eólico com 3 tipos de sensores: Medidor de Potência, Temperatura e Pressão Hidráulica. E por meio de dados gerados por Python, extrair e coletar os dados para análise dentro do AWS utilizando o Athena AWS. 

O esquema de ferramentas utilizadas pode ser observado na seguinte imagem:

![image](https://user-images.githubusercontent.com/66450718/208470365-2d098d40-f316-45bf-825b-2494bcfae236.png)

## Passo-a-Passo do Projeto

Para realizar ao atividades proposta, utilizou-se da seguinte estrutura:
 
* Criação de Arquivos em Python para criação de dados de: Potência, Temperatura e Pressão Hidráulica em formato JSON;
* Criação do Kinesis Data Stream para captação dos dados advindos Python Notebook;
* Utilização do Kinesis Data Firehouse para redirecionamento dos dados para um Bucket no S3;
* Aplicação de Crawler e IAM para mapeamento das tables criadas no Bucket do S3;
* Criação do Glue Catalog e dos Jobs pelo Glue para comprimir os arquivos de dados gerados para o formato parquet e lançar para outro Bucket no S3;
* Utilização de outro Crawler para leitura das Tables dos dados em Parquet e análise do banco de dados com o AWS Athena.


_______
## Referências

Link do curso: <https://www.udemy.com/course/engenheiro-de-dados/>

Gabriel de Oliveira Dantas --- [Linkedin](https://www.linkedin.com/in/gabriel-dantas2/)
