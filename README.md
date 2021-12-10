# desafio-dio-dremio
Desafio da DIO:  Criando seu Primeiro Repositório no GitHub Para Compartilhar Seu Progresso

# Instalação do Dremio on premisse no Docker. 

<p align="center"><img src="./dremio-logo-dark.png" width="500"></p>

## O que é o Dremio?

Dremio é uma plataforma de dados como um serviço (Data-as-a-Service) que capacita os usuários para descobrir, curar, acelerar e compartilhar quaisquer dados a qualquer momento, independentemente da localização, volume ou estrutura. Use sua ferramenta de BI favorita, linguagem Python, R e outras ferramentas baseadas em SQL para acessar dados de qualquer fonte. Use Dremio para manter um catálogo central e pesquisável de todos os seus conjuntos de dados, crie e execute um ETL que funcione em seus dados, acelere consultas usando Data Reflections e misture dados entre fontes, incluindo sistemas que não suportam SQL, como ElasticSearch, MongoDB e S3.

Os fundadores da Dremio também são os co-criadores da Apache Arrow, uma plataforma para processamento colunar em memória. Apache Arrow é usada extensivamente pela Dremio e é núcleo para muitos outros projetos de código aberto. Leia mais sobre a origem e história do Apache Arrow: https://www.dremio.com/origin-history-of-apache-arrow/

__*Vantagem do Dremio*__

Dremio torna muito simples executar consultas SQL diretamente no seu Data Lake na nuvem sem fazer cópias dos seus dados.

---

## Container do Docker

Dremio - open source Data-as-a-Service Platform (community edition).  

### 1. Docker Pull Command

Para criar a image do container, executar o comando:

``` bash
docker pull dremio/dremio-oss 
```

### 2. Para subir o container (single node)

O container ficará executando e o Dremio ficará disponível no seu browser de preferência na porta 9047:

```bash
docker run -p 9047:9047 -p 31010:31010 -p 45678:45678 dremio/dremio-oss
```
Assim, 

```html
http://localhost:9047
```

Estão inclusos e devidamente configurados:
* Embedded Zookeeper
* Master Coordinator
* Executor

---

## Missão Cumprida
Se tudo estiver certo, você verá a seguinte tela de boas-vindas:

<p align="center"><img src="./dremio-logo-dark.png" width="500"></p>
