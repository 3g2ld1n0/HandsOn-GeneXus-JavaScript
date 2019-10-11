# Atividade 09

Nesta atividade vamos mostrar a criação de um User Control.

## Semantic UI

Da mesma forma que o BootStrap o **Semantic UI** possui uma série de componentes para agilizar o desenvolvimento.

## Exercício

Vamos conhecer uma nova funcionalidade bem legal do GeneXus e também um novo framework.

No site https://semantic-ui.com você pode visualizar todos os componentes, inclusive baixar os arquivos para usar.

## User Control GeneXus

Agora criar controles com belas apresentações no GeneXus ficou mais fácil. Com esses controles podemos usar os layouts, adicinando propriedades.

Assim os controles poderam ser usados de modo nativo dentro do GeneXus.

Como fonte de dados, vamos utilizar uma API pública que não precisa de registro https://swapi.co, mas para facilitar vamos baixar o arquivo e importar para a nossa KB.

- [Atividade9.zip](https://github.com/3g2ld1n0/HandsOn-GeneXus-JavaScript/blob/master/Arquivos/Atividade09.zip)

Vamos criar um novo objeto e nomea-lo de **PeopleUC**

![User Control](/Image/Requisitos20.png)

A próxima etapa consiste em colocar dentro do controle o código **HTML** e **JavaScript** necessários para o controle.

No site do vamos fazer o uso do **Cars** https://semantic-ui.com/views/card.html

![Card Group](/Image/Requisitos21.png)

O código exemplo possui 3 cards dentro de um objeto agrupador, mas para nosso exemplo vamos colocar e um, e fazer ele se repetir.

```HTML
<script src="https://semantic-ui.com/dist/semantic.min.js"></script>
<link rel="stylesheet" type="text/css" class="ui" href="https://semantic-ui.com/dist/semantic.min.css">

<div class="ui link cards">
  <div class="card">
    <div class="image">
      <img src="https://semantic-ui.com/images/avatar2/large/matthew.png">
    </div>
    <div class="content">
      <div class="header">name</div>
      <div class="meta">
        <a>Details</a>
      </div>
      <div class="description">
	  	name Hair Color hair_color Bird Year birth_year Gender gender.
      </div>
    </div>
    <div class="extra content">
      <span class="right floated">
        Height height
      </span>
      <span>
        <i class="user icon"></i>
        Eye color eye_color
      </span>
    </div>
  </div>
</div>
```

O SDT dos dados é esse, agora precisamos preparar o User Control para receber a parte variável.

![SDT Dados](/Image/Requisitos22.png)

Com esse código estamos criando:
- **{{#results}}** e **{{/results}}** é responsável para fazer um looping dos dados de coleção no SDT.
- **{{name}}**, **{{hair_color}}**, **{{birth_year}}**, **{{gender}}** e etc. São as proriedades dentro da coleção.

Quando executado o User Control uma macro substituição será executada.

```HTML
<script src="https://semantic-ui.com/dist/semantic.min.js"></script>
<link rel="stylesheet" type="text/css" class="ui" href="https://semantic-ui.com/dist/semantic.min.css">


<div class="ui link cards">
  {{#results}}
  <div class="card">
    <div class="image">
      <img src="https://semantic-ui.com/images/avatar2/large/matthew.png">
    </div>
    <div class="content">
      <div class="header">{{name}}</div>
      <div class="meta">
        <a>Details</a>
      </div>
      <div class="description">
	  	{{name}} hair color {{hair_color}} bird year {{birth_year}} gender {{gender}}.
      </div>
    </div>
    <div class="extra content">
      <span class="right floated">
        Height {{height}}
      </span>
      <span>
        <i class="user icon"></i>
        Eye color: {{eye_color}}
      </span>
    </div>
  </div>
  {{/results}}
</div>
```

O **Screen Template** deve ficar assim

![Screen Template](/Image/Requisitos23.png)

O **Properties** deve ficar assim, propriedades relevantes são **results** e **resultsCurrentIndex** uma para coleção e outra para o índice.

![Properties](/Image/Requisitos24.png)

No WebPanel criado vamos adicionar o nosso controle criado **PeopleUC**. 

![Adicionar Controle](/Image/Requisitos25.png)

E fazer a chamada para a WebAPI

![Chamar API](/Image/Requisitos26.png)

Associar lista para o User Control

![Associar Lista](/Image/Requisitos27.png)

O que nos resta é executar o WebPanel e ver o resultado final.