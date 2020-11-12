# Criando migração no MongoDB com Liquibase

## Pré requisitos

É necessário ter o Java instalado e configurado

1. Baixar o [liquibase-4.1.1.tar.gz](https://www.liquibase.org/download) e descompactar

2. Instalar o [Liquibase](https://docs.liquibase.com/concepts/installation/home.html):

```
  $ export PATH=$PATH:/path/to/Liquibase-<version>-bin

  $ source ~/.profile 
  OU
  $ source ~/.bashrc
  
``` 
3. Testar se está configurado corretamente:

```
  $ liquibase --help
  
```

4. Baixar o [driver jdbc para Mongo](https://repo1.maven.org/maven2/org/mongodb/mongo-java-driver)

  - mongo-java-driver-3.9.1.jar

5. Baixar o [arquivo jar](https://github.com/liquibase/liquibase-mongodb/releases/tag/liquibase-mongodb-4.0.0.2) de extensão para o Liquibase

  - liquibase-mongodb-4.0.0.2.jar

6. Salvar os dois arquivos jar na pasta /lib, onde foi instalado o Liquibase

## Tutorial

1. Criar a pasta que conterá o projeto

2. Nesta pasta, criar o arquivo dbchangelog.xml com as instruções de migração

3. Nesta mesma pasta, criar o arquivo liquibase.properties com as configurações do Mongo

4. No diretório do projeto, executar o comando:

  $ liquibase update
  
  
## Outras ferramentas para migração Mongo

[mongobee](https://github.com/mongobee/mongobee) 

[mongol](https://github.com/coldze/mongol)

[mongeez](https://github.com/mongeez/mongeez)

[node-migrate](https://github.com/tj/node-migrate)

[Mongration](https://github.com/KuliginStepan/mongration)


## Certificação Liquibase

[Liquibase Fundamentals Certification](https://learn.liquibase.com/catalog/info/id:125)


## Referências

[Using the Liquibase Installer](https://www.liquibase.org/get-started/using-the-liquibase-installer)

[Using Liquibase with MongoDB](https://docs.liquibase.com/workflows/database-setup-tutorials/mongodb.html)

[Liquibase MongoDB Extension](https://github.com/liquibase/liquibase-mongodb)
  


  
