---
layout: default
---

Text can be **bold**, _italic_, ~~strikethrough~~ or `keyword`.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Sobre o Spotify

Quando o Spotify foi lançado em 2008, a indústria musical sofreria mudanças abruptas e adaptações na forma como se consome e se comercializa música - sendo ela por parte de artistas, consumidores ou produtores. Atualmente com mais de 100 milhões de faixas e 5 milhões de episódios de Podcasts, considerando que o consumidor pode usufruí-los a partir de um plano gratuito ou pago, que conta com qualidade de som aprimorada e uma experiência de sessão mais completa, podendo escutar qualquer título mesmo offline, o Spotify é, sem dúvidas, o serviço de streaming musical mais popular, ainda mais que o Apple Play, contando com mais de 500 milhões de usuários registrados e 205 milhões de assinantes em mais de 180 países.

O modelo de negócios da plataforma se baseia na venda de assinaturas premium e na exibição de anúncios para os usuários que usufruem do plano mais básico. Além disso, também funciona como uma forma de complemento de renda aos artistas, além de permitir que suas obras alcancem mais destaque e público - o que se dá principalmente a partir do sistema de recomendações da plataforma e das playlists públicas. A cada dez plays em alguma faixa, o Spotify repassa US$ 0,04 ao artista ou a sua gravadora 


## Arquitetura

Quando em janeiro de 2023 o cantor canadense Abel Makkonen, conhecido como The Weeknd, ultrapassou a marca dos 93 milhões de ouvintes mensais na plataforma, ultrapassando nomes como Ed Sheeran (86m) e Taylor Swift (81.21m), quebrando o recorde prévio da plataforma e sendo estabelecido como o maior nome da indústria por determinado tempo, deve-se pensar nas características internas do Spotify; isso é, sua arquitetura e suas peculiaridades que permitem com que tantos usuários utilizem a plataforma simultânea e periodicamente sem que o sistema colapse mediante a esses números. Nesse ponto, vale também considerar que o Spotify possui uma versão Web, uma Desktop e outra APK.

## Microsserviços

A arquitetura do Spotify é baseada em microsserviços, como explicado por Kevin Goldsmith, CTO da empresa. Em suma, uma arquitetura de microsserviços implica na separação independente de serviços/componentes, cada qual com sua funcionalidade específica, o que facilita em quesitos de desenvolvimento de software como manutenabilidade, escalabilidade, desempenho, etc.
O Spotify está entre as empresas pioneiras na utilização de microsserviços e no aproveitamento de seus inúmeros benefícios, permitindo que a plataforma desenvolva e disponibilize novas funcionalidades periodicamente, visto que cada serviço ou funcionalidade estão contidos em módulos específicos. A escolha desse modelo arquitetural também auxilia o Spotify a lidar com enormes volumes de dados e requisições, além de possibilitar a atuação de várias equipes em diferentes serviços. Dessa forma, é correto dizer que a escolha arquitetural implicou na popularidade e sucesso da empresa e do serviço.

O backend do Spotify necessita de inúmeros serviços/módulos, como verificação de usuário, recomendação de músicas, sistema de pesquisa, entre outros.

![image](https://github.com/Luiz-Gustavo-SS/TP-ArqSoftware/assets/84593164/bcf90a62-96fb-4d8c-8394-de17e417c043)


![image](https://github.com/Luiz-Gustavo-SS/TP-ArqSoftware/assets/84593164/f353ba2d-f22b-45ad-b569-596c14bdc8d4)


## Tecnologias

Geralmente esses serviços são escritos em Python e Java e se comunicam entre si via protocólo Hermes, desenvolvido pela própria empresa.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
