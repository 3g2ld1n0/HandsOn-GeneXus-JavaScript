# Atividade 07

Nesta atividades vamos juntar o que vimos até agora com uma KB GeneXus.

## Exercício

Baixe o arquivo atividade7.zip, nele vamos usar o arquivo **XPZ** para criar a base de conhecimento.

E vamos copiar o arquivo **Util.js** para uma pasta **WEB\TypeScript\**

- [Atividade7.zip](https://github.com/3g2ld1n0/HandsOn-GeneXus-JavaScript/blob/master/Arquivos/Atividade07.zip)

Com a aplicação rodando vamos criar alguns registros e fazer o uso do nosso arquivo JS.

## JavaScript no Cliente

Para adicionar o arquivo JavaScript ao webpanel **WWCliente** faremos da seguinte forma.

Colocando no **Start** do objeto a linha **Form.JScriptSrc.Add('TypeScript/Util.js')**.

Em seguida vamos fazer a chamada do **ViewCliente** usando a função **OpenPopUP** que está no arquivo JavaScript.

Adicionando no evento **Grid.Load** a seguinte linha **&View.Link = "JavaScript:OpenPopUP('" + ViewCliente.Link(ClienteId, "") + "', 800, 200);"**

Executando a aplicação vermos que a nova janela será aberta sem nenhuma chamada ao servidor.

## JavaScript no Calculo

Para adicionar o arquivo JavaScript ao webpanel **Calcular** faremos da seguinte forma.

Colocando no **Start** do objeto a linha **Form.JScriptSrc.Add('TypeScript/Util.js')**.

Ainda no **Start** vamos adicionar a seguinte linha **imgOK.Link = "JavaScript:Calcular($('#" + &Valor1.InternalName + "').val(), $('#" + &Valor2.InternalName + "').val());"**

Executando a aplicação devemos preencher os valores e ver o resultado do calculo.

Próxima atividade: [Atividade 08](ATIVIDADE08.md)