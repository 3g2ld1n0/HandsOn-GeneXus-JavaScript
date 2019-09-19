# Atividade 01
Para esta atividade vamos começar a ver na prática o que faz o JavaScript

## Visual Code

Vamos criar uma pasta de trabalho chamada **HandsOn-GeneXus-JavaScript** na unidade "C:\"

Abrindo o Visual Code, vamos selecionar essa pasta criada. Para isso escolha a opção **File** e em seguida **Open Folder**

![Abrir Pasta](/Image/Requisitos05.png)

Escolha a pasta criada e clique em **Select Folder**

![Escolher Pasta](/Image/Requisitos06.png)

Crie um arquivo selecionando a opção **1** em seguida nomeando-o **Atividade01.html** conforme opção **2** e tecle **Enter**

![Criando arquivo](/Image/Requisitos07.png)

Copie o seguinte código para o arquivo e salve

```html
<!DOCTYPE html>
<html>

<body>
    <h2>O que o JavaScript pode fazer?</h2>
    <h3>JavaScript pode mudar os valores dos atributos HTML.</h3>
    <div>
        <h2>Nesse caso JavaScript muda o atributo src(source) de uma imagem.</h2>
        <button onclick="document.getElementById('myImage').src='pic_bulbon.gif'">Ligar</button>
        <img id="myImage" src="pic_bulboff.gif" style="width:100px">
        <button onclick="document.getElementById('myImage').src='pic_bulboff.gif'">Desligar</button>
    </div>

    <div>
        <h2>Nesse caso apresentamos a Data e Hora</h2>
        <button type="button" onclick="document.getElementById('demo').innerHTML = Date()">Clique para exibir a data e
            hora.</button>
        <p id="demo"></p>
    </div>

    <div>
        <h2>Nesse caso será alterado o estilo</h2>
        <p id="demo2">JavaScript pode mudar os valores dos atributos HTML.</p>
        <button type="button" onclick="document.getElementById('demo2').style.fontSize='35px'">Clique!</button>
    </div>

    <div>
        <h2>Neste caso será escondido/exibido</h2>
        <p id="demo3">JavaScript pode mudar os valores dos atributos HTML.</p>
        <button type="button" onclick="document.getElementById('demo3').style.display='none'">Esconder</button>
        <button type="button" onclick="document.getElementById('demo3').style.display='block'">Exibir</button>
    </div>

    <div>
        <h2>Neste caso será efetuado um calculo</h2>
        <p>JavaScript pode mudar os valores dos atributos HTML.</p>
        <span>O resultado (0.2*10 + 0.1*10) / 10 = </span>
        <span id="demo4">?</span>
        <p></p>
        <button type="button"
            onclick="document.getElementById('demo4').innerHTML = (0.2*10 + 0.1*10) / 10">Calcular</button>
    </div>

</body>

</html>
```

Fazer o download do arquivo atividade1.zip. Descompactar e copiar os arquivos para a pasta **C:\HandsOn-GeneXus-JavaScript**

- [Atividade1.zip](https://github.com/3g2ld1n0/HandsOn-GeneXus-JavaScript/blob/master/Arquivos/Atividade01.zip)

Abra o arquivo HTML criado e vamos ver o resultado

Próxima atividade: [Atividade 02](ATIVIDADE02.md)