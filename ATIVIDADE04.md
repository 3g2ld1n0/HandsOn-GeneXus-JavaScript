# Atividade 04
Nesta atividade vamos pegar o primeiro arquivo de exercício, salvar como Atividade04.html. E criar funções para todos os eventos que estão ligados diretos aos elementos HTML.

## Resolução

Arquivo JavaScript proposta como solução **Atividade04.js**

```JavaScript
var ligado = false;
var exibir = true;
function Interruptor() {
    ligado = !ligado;
    if (ligado == true) {
        document.getElementById('btInterruptor').innerText = 'Desligar';
        document.getElementById('myImage').src = 'pic_bulbon.gif';
    } else {
        document.getElementById('btInterruptor').innerText = 'Ligar';
        document.getElementById('myImage').src = 'pic_bulboff.gif';
    }
}

function DataGet() {
    document.getElementById('demo1').innerHTML = Date();
}

function MudarEstilo() {
    document.getElementById('demo2').style.fontSize = '35px';
}

function MudarEstilo2(objetoId) {
    document.getElementById(objetoId).style.fontSize = '35px';
}

function ExibirEsconder() {
    exibir = !exibir;
    if (exibir == true) {
        document.getElementById('demo4').style.display = 'block';
    } else {
        document.getElementById('demo4').style.display = 'none';
    }
}
```

Arquivo HTML proposta como solução **Atividade04.html**

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
    <script src="atividade04.js"></script>
</head>

<body>
    <div class="container">
        <h2>O que o JavaScript pode fazer?</h2>
        <span>JavaScript pode mudar os valores dos atributos HTML.</span>
        <div class="panel-group">
            <div class="panel panel-default">
                <div class="panel-heading">Nesse caso JavaScript muda o atributo src(source) de uma imagem.</div>
                <div class="panel-body">
                    <img id="myImage" src="pic_bulboff.gif" style="width:100px"><br /><br />
                    <button class="btn btn-primary" onclick="Interruptor()" id="btInterruptor">Ligar</button>
                </div>

            </div>

            <div class="panel panel-primary">
                <div class="panel-heading">Nesse caso apresentamos a Data e Hora</div>
                <div class="panel-body">
                    <button class="btn btn-primary" type="button" onclick="DataGet()">Clique para exibir a data e
                        hora.</button>
                    <span id="demo1">(id=demo1)</span>
                </div>
            </div>

            <div class="panel panel-success">
                <div class="panel-heading">Nesse caso será alterado o estilo</div>
                <div class="panel-body">
                    <p id="demo2">JavaScript pode mudar os valores dos atributos HTML. (id=demo2)</p>
                    <button class="btn btn-primary" type="button" onclick="MudarEstilo()">Clique!</button>
                </div>
            </div>

            <div class="panel panel-info">
                <div class="panel-heading">Nesse caso será alterado o estilo</div>
                <div class="panel-body">
                    <div class="form-group">
                        <label for="IdObjeto">Id Objeto:</label>
                        <input type="text" id="objetoId" class="form-control" value="" placeholder="Digite Id Objeto" />
                        <p id="demo3">JavaScript pode mudar os valores dos atributos HTML com parâmetros. (id=demo3)</p>
                        <button class="btn btn-primary" type="button"
                            onclick="MudarEstilo2(document.getElementById('objetoId').value)">Clique!</button>
                    </div>
                </div>
            </div>

            <div class="panel panel-warning">
                <div class="panel-heading">Neste caso será escondido/exibido</div>
                <div class="panel-body">
                    <button class="btn btn-primary" type="button" onclick="ExibirEsconder()">Esconder/Exibir</button>
                    <p id="demo4">JavaScript pode mudar os valores dos atributos HTML. (id=demo4)</p>
                </div>
            </div>

            <div class="panel panel-danger">
                <div class="panel-heading">Neste caso será efetuado um calculo</div>
                <div class="panel-body">
                    <p>JavaScript pode mudar os valores dos atributos HTML.</p>
                    <span>O resultado (0.2*10 + 0.1*10) / 10 = </span></br>
                    <span id="demo5">?</span></br>
                    <p></p>
                    <button class="btn btn-primary" type="button"
                        onclick="document.getElementById('demo5').innerHTML = (0.2*10 + 0.1*10) / 10">Calcular</button>
                </div>
            </div>
        </div>
    </div>
</body>

</html>
```

Próxima atividade: [Atividade 05](ATIVIDADE05.md)

