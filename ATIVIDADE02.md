# Atividade 02
Nesta atividade vamos organizar melhor o código JavaScript, colocando em áreas específicas no documento/arquivo HTML.

## Cabecalho (Head)

No HTML, o JavaScript deve ser colocado entre as tags <script> e </script>.

Neste exemplo, a função JavaScript é adicionada no seção <head> da página HTML.

A função é chamada quando o botão é clicado.

Crie um novo arquivo chamado de **Atividade02a.html** e copiei o código a seguir.

```html
<!DOCTYPE html>
<html>
<head>
<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "Paragraph changed.";
}
</script>
</head>
<body>

<h1>A Web Page</h1>
<p id="demo">A Paragraph</p>
<button type="button" onclick="myFunction()">Try it</button>

</body>
</html>
```

Abra o arquivo HTML criado e vamos ver o resultado.

## Corpo (Body)

Neste exemplo, a função JavaScript é adicionada no seção <body> da página HTML.

A função é chamada quando o botão é clicado.

Crie um novo arquivo chamado de **Atividade02b.html** e copiei o código a seguir.

```html
<!DOCTYPE html>
<html>
<body>

<h1>A Web Page</h1>
<p id="demo">A Paragraph</p>
<button type="button" onclick="myFunction()">Try it</button>

<script>
function myFunction() {
 document.getElementById("demo").innerHTML = "Paragraph changed.";
}
</script>

</body>
</html>
```

Abra o arquivo HTML criado e vamos ver o resultado.

Próxima atividade: [Atividade 03](ATIVIDADE03.md)