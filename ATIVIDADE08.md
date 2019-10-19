# Atividade 08

Nesta atividade vamos fazer criar as mesmas rotinas usando TypeScript e External Objects for JavaScript dentro do GeneXus, usando uma abordagem diferente.

**Documentação GeneXus** https://wiki.genexus.com/commwiki/servlet/wiki?31064,External+Objects+for+Javascript#targetText=The%20JavaScript%20External%20Name%20property,defined%20in%20the%20JS%20code.

## Exercício

Usando o **Visual Code** vamos abrir a pasta da **WEB\TypeScript** da KB.

Agora vamos criar um novo arquivo chamado **UtilEO.ts** e adicionar o seguinte código.

```TypeScript
class Janela {
    Abrir(url:string, nomeJanela:string, largura:string, altura:string) {
        window.open(url, nomeJanela, 'width=' + largura + ',height=' + altura);
    }
}

class Calculadora {
    public Valor1: number = 0;
    public Valor2: number = 0;
    public Resultado: number = 0;

    Soma():void {
        this.Resultado = this.Valor1 + this.Valor2;
    }

}
```
Abrindo a linha de comando no Visual Code vamos executar o comando **tsc UtilEO.ts**. O resultado é um novo arquivo será criado com o nome **UtilEO.js**.

O arquivo JavaScript deve ser adicionado nos Webpanels da mesma forma que atividade anterior.

Para usar esse novo arquivo em nossa base de conhecimento vamos criar um objeto externo chamado **JanelaEO**

![Objeto Externo](/Image/Requisitos17.png)

Em sua propriedade **Javascript External Name** vamos preencher com o nome do objeto que está no arquivo javascript **Janela**

![Objeto Externo](/Image/Requisitos18.png)

Agora vamos adicionar a método da classe **Abrir** com seus parâmetros **url**, **nomeJanela**, **largura**, **altura** conforme imagem.

O método deve ser configurado como estático, e na **Javascript External Name** vamos preencher com o nome método o que está no arquivo javascript **Abrir**

![Objeto Externo](/Image/Requisitos19.png)

Com estes passos mapeamos o popup no objeto externo, agora vamos usar em nosso grid de clientes adicionando um novo botão e fazendo o uso do mesmo.

Para concluirmos essa atividade vocês devem criar o objeto externo para calcular e aplicar na tela.

Bonus atividade: [Atividade 09](ATIVIDADE09.md)