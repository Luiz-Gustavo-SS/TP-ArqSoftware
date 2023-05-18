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

O backend do Spotify necessita de inúmeros serviços/módulos, como verificação de usuário, recomendação de músicas, sistema de pesquisa, entre outros.

![image](https://github.com/Luiz-Gustavo-SS/TP-ArqSoftware/assets/84593164/f353ba2d-f22b-45ad-b569-596c14bdc8d4)


## Tecnologias

Geralmente esses serviços são escritos em Python e Java e se comunicam entre si via protocólo Hermes, desenvolvido pela própria empresa.
O Python é utilizado no back-end, scripts, processos e análise de dados, e aproximadamente 80% dos serviços da plataforma são escritos no mesmo.
