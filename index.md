---
layout: default
---
# Sobre o Spotify

Quando o Spotify foi lançado em 2008, a indústria musical sofreria mudanças abruptas e adaptações na forma como se consome e se comercializa música - sendo ela por parte de artistas, consumidores ou produtores. Atualmente com mais de 100 milhões de faixas e 5 milhões de episódios de Podcasts, considerando que o consumidor pode usufruí-los a partir de um plano gratuito ou pago, que conta com qualidade de som aprimorada e uma experiência de sessão mais completa, podendo escutar qualquer título mesmo offline, o Spotify é, sem dúvidas, o serviço de streaming musical mais popular, ainda mais que o Apple Play, contando com mais de 500 milhões de usuários registrados e 205 milhões de assinantes em mais de 180 países.

O modelo de negócios da plataforma se baseia na venda de assinaturas premium e na exibição de anúncios para os usuários que usufruem do plano mais básico. Além disso, também funciona como uma forma de complemento de renda aos artistas, além de permitir que suas obras alcancem mais destaque e público - o que se dá principalmente a partir do sistema de recomendações da plataforma e das playlists públicas. A cada dez plays em alguma faixa, o Spotify repassa US$ 0,04 ao artista ou a sua gravadora 


## Arquitetura

Quando em janeiro de 2023 o cantor canadense Abel Makkonen, conhecido como The Weeknd, ultrapassou a marca dos 93 milhões de ouvintes mensais na plataforma, deve-se pensar nas características internas do Spotify; isso é, sua arquitetura e suas peculiaridades que permitem com que tantos usuários utilizem a plataforma simultânea e periodicamente sem que o sistema colapse mediante a esses números. Nesse ponto, vale também considerar que o Spotify possui uma versão Web, uma Desktop e outra APK, que se comunicam entre si.
A plataforma também possui uma arquitetura separada para cuidar das questões relacionadas a assinaturas e pagamentos:

![image](https://github.com/Luiz-Gustavo-SS/TP-ArqSoftware/assets/84593164/aa0295cd-8dd7-4a8b-a1c5-82fc87972adb)


## Microsserviços

A arquitetura do Spotify é baseada em microsserviços, como explicado por Kevin Goldsmith, CTO da empresa. Em suma, uma arquitetura de microsserviços implica na separação independente de serviços/componentes, cada qual com sua funcionalidade específica, o que facilita em quesitos de desenvolvimento de software como manutenabilidade, escalabilidade, desempenho, etc.
O Spotify está entre as empresas pioneiras na utilização de microsserviços e no aproveitamento de seus inúmeros benefícios, permitindo que a plataforma desenvolva e disponibilize novas funcionalidades periodicamente, visto que cada serviço ou funcionalidade estão contidos em módulos específicos. A escolha desse modelo arquitetural também auxilia o Spotify a lidar com enormes volumes de dados e requisições, além de possibilitar a atuação de várias equipes em diferentes serviços. Dessa forma, é correto dizer que a escolha arquitetural implicou na popularidade e sucesso da empresa e do serviço.

## Backend 

O Spotify utiliza um sistema de backend distribuído para garantir que as solicitações dos usuários sejam processadas de forma eficiente. Os microsserviços se comunicam entre si por meio de APIs, trocando dados e coordenando suas atividades. Essa arquitetura distribuída permite que o Spotify dimensione horizontalmente seus recursos, adicionando mais servidores conforme necessário, para lidar com o crescimento da base de usuários e a demanda.

## Algoritmos de Recomendação

Um dos pontos fortes do Spotify é seu recurso de recomendação de música personalizada. Isso é possível graças a algoritmos avançados que analisam o histórico de escuta do usuário, seus gostos musicais, preferências e dados demográficos para oferecer sugestões relevantes. Esses algoritmos operam em um sistema de aprendizado de máquina que é alimentado continuamente com dados atualizados para refinar ainda mais as recomendações.

## Nas alturas

O Spotify utiliza serviços em nuvem, como o Google Cloud Platform (GCP) e o Amazon Web Services (AWS), para hospedar sua infraestrutura. Essa abordagem permite que o Spotify dimensione seus recursos rapidamente e forneça uma alta disponibilidade dos serviços em todo o mundo, garantindo elasticidade e flexibilidade.

![image](https://github.com/Luiz-Gustavo-SS/TP-ArqSoftware/assets/84593164/f353ba2d-f22b-45ad-b569-596c14bdc8d4)


## Tecnologias

Geralmente esses serviços são escritos em Python e Java e se comunicam entre si via protocólo Hermes, desenvolvido pela própria empresa.
O Python é utilizado no back-end, scripts, processos e análise de dados, e aproximadamente 80% dos serviços da plataforma são escritos no mesmo.

## Protocolo Hermes 

O Protocolo Hermes, desenvolvido internamente pelo Spotify, é um conjunto de tecnologias e algoritmos projetados para aprimorar a qualidade do streaming de áudio. Ele foi criado com o objetivo de reduzir a latência, minimizar interrupções e garantir uma reprodução fluida das músicas, independentemente da qualidade da conexão de Internet do usuário.  
Um dos principais desafios enfrentados pelo Spotify e outros serviços de streaming de música é a variação na qualidade da conexão à Internet dos usuários. Alguns usuários podem ter acesso rápido e estável à Internet, enquanto outros podem enfrentar conexões lentas, instáveis ou com perda de pacotes. O Protocolo Hermes foi desenvolvido para lidar com essas variações e fornecer uma experiência consistente, independentemente da qualidade da conexão.  
Uma das técnicas utilizadas pelo Protocolo Hermes é o armazenamento em buffer inteligente. Ele monitora constantemente a velocidade da conexão à Internet do usuário e ajusta dinamicamente o tamanho do buffer de áudio para garantir uma reprodução contínua. Se a velocidade da conexão diminuir temporariamente, o buffer será dimensionado adequadamente para evitar interrupções na reprodução. Isso permite que os usuários aproveitem suas músicas sem interrupções irritantes.

## Referências

https://engineering.atspotify.com/
https://www.techaheadcorp.com/blog/decoding-software-architecture-of-spotify-how-microservices-empowers-spotify/
https://www.godeltech.com/is-spotify-the-holy-grail-of-software-engineering/
