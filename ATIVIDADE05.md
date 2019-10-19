# Atividade 05

Nesta atividade vamos entender, o valor do TypeScript para o nosso dia a dia.

## Exercício

Vamos criar um novo arquivo chamado **Atividade05.html**, em seguida copiar o código a abaixo.

```html
<!DOCTYPE html>
<html>

<head>
    <title>Bootstrap Example</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/js/bootstrap.min.js"></script>
    <script src="Atividade05.js"></script>
</head>

<body>
    <div class="container">
        <h2>O que o TypeScript pode fazer?</h2>
        <p>Pressione F12 e acompanhe no console o resultado dos scripts</p>
    </div>
</body>

</html>
```

Em seguida vamos criar um novo arquivo chamado **Atividade05.js** e lá vamos adicionar o código JavaScript.

```JavaScript
console.log('Exibindo valores');

console.log('--- Soma ---');
a = 1;
b = 2;
c = a + b;
console.log('a =', a);
console.log('b =', b);
console.log('(a + b) = c =', c);

console.log('--- Subitracao ---');
a = 1;
b = 2;
c = a - b;
console.log('a =', a);
console.log('b =', b);
console.log('(a + b) = c =', c);

console.log('--- Concatenacao ---');
a = 'Jose';
b = 'Lima';
c = a + b;
console.log('a =', a);
console.log('b =', b);
console.log('(a + b) = c =', c);

console.log('--- Objeto ---');
carro = { nome:'Gol', fabricante:'VW' };
console.log('carro.nome =', carro.Nome);
console.log('carro.fabricante =', carro.Fabricante);

console.log('--- Comparação ---');
a = 10;
if (a == 10){
    console.log('O valor de "a" eh:', a);
}

if (a == '10'){
    console.log('O valor de "a" eh:', a);
}

console.log('--- Arrays to string ---');
ferramentas = ['Visual Studio', 'Visual Code', 'GeneXus', 'TypeScript'];
console.log(ferramentas.ToString());

console.log('--- Arrays to join ---');
ferramentas = ['Visual Studio', 'Visual Code', 'GeneXus', 'TypeScript'];
console.log(ferramentas.Join(';'));
```
Antes de abrir o arquivo podemos dizer o que será executado para cada console?

Conseguimos dizer o que está errado?

Vamos abrir o arquivo no navegador e ver o resultado no console.

Próxima atividade: [Atividade 06](ATIVIDADE06.md)