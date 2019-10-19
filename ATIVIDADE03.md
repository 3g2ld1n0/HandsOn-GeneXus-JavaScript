# Atividade 03
Nesta atividade continuamos a organizar melhor o código JavaScript no documento/arquivo HTML.

Também vamos utilizar de novos recursos de extrema importancia para o desenvolvimento WEB.

## Bootstrap

O Bootstrap é uma ferramenta gratuita para desenvolvimento HTML, CSS e JS. Crie protótipos rápidamente ou aplicações completas com nossas variáveis e mixins Sass, sistemas de grid responsivo, componentes pré-construídos e poderosos plugins com jQuery.

Aqui [Bootstrap](https://getbootstrap.com/) pegamos as informações necessárias para o uso. 

![Bootstrap](/Image/Requisitos08.png)

Mas por hora, vamos exibir um código na atividade que já mostra a inclusão dos **CSS** e **Scripts** necessários.

## Exercício

O código a seguir mostra outra forma de organizar os scripts e arquivos de estilos.

```HTML
<head>
    <title>Bootstrap Example</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/js/bootstrap.min.js"></script>
</head>
```

Na tag **link** e **script** estamos adicionado os arquivos de estilo CSS e script JS. Desta forma os códigos não ficaram na página, facilitando nossa vida quando necessário leva-los para outras páginas no desenvolvimento.

Uma das tags **meta** a de nome **viewport** é adicionada para trabalhar na com a parte responsiva da página que será cuidada pelo Bootstrap.

Crie um novo arquivo **Atividade03.html** e copie todo o código.

```HTML
<!DOCTYPE html>
<html>

<head>
    <title>Bootstrap Example</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/js/bootstrap.min.js"></script>
</head>

<body>
    <div class="container">
        <h2>JavaScript Variables</h2>
        <p>In this example, x, y, and z are variables.</p>
        <p>x = 5, y = 6</p>
        <p></p>
        <p id="demo1"></p>

        <p>The result of adding "5" + 2 + 3:</p>
        <p id="demo2"></p>

        <p>The result of adding 2 + 3 + "5":</p>
        <p id="demo3"></p>

        <h2>JavaScript Objects</h2>
        <p>The .table-bordered class adds borders to a table:</p>
        <table class="table table-bordered">
            <thead>
                <tr>
                    <th>Type</th>
                    <th>Model</th>
                    <th>Color</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td><span id="type"></span></td>
                    <td><span id="model"></span></td>
                    <td><span id="color"></span></td>
                </tr>
            </tbody>
        </table>
    </div>

    <script>
        var x = 5;
        var y = 6;
        var z = x + y;
        document.getElementById("demo1").innerHTML =
            "The value of z is: " + z;

        x = "5" + 2 + 3;
        document.getElementById("demo2").innerHTML = x;

        var x = 2 + 3 + "5"
        document.getElementById("demo3").innerHTML = x;

        // Create an object:
        var car = { type: "Fiat", model: "500", color: "white" };

        // Display some data from the object:
        document.getElementById("type").innerHTML = car.type;
        document.getElementById("model").innerHTML = car.model;
        document.getElementById("color").innerHTML = car.color;
    </script>

</body>

</html>
```

Quando abrir o arquivo no navegador, vamos inspencionar o documento. Para isso pressione **F12** e se você fizer isso no navegador Google Chrome deve ter esse resultado.

Clique na opção **Elements** e vamos poder acessar os códigos conforme imagem. Em destaque as classes do Bootstrap.

![F12 Navegador](/Image/Requisitos09.png)

Usando esse recurso dos navegadores, podemos realizar ajustes durante a execução e leva-los para código final. Como exemplo disso vamos trocar a classe atual **info** para **success**, para modificar basta clicar duas vezes na classe.

### Variáveis

Não menos importante :), podemos perceber na área de script as varíaveis. 

![Variáveis](/Image/Requisitos10.png)

Exemplos de criação de váriaveis.

![Variáveis](/Image/Requisitos11.png)

### Dicas  
Notem que para o JavaScript existe uma situação que a ordem dos "Tratores" sim, altera o "Viaduto". 

E trabalhando com desenvolvimento web, não importa o código que você está escrevendo, mas sim o que foi gerado.

Próxima atividade: [Atividade 04](ATIVIDADE04.md)