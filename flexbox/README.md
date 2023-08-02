# Flexbox
Flexbox é um módulo do CSS que permite criar **layouts flexíveis e responsivos** em uma página da Web. Ele permite que você controle a posição, o tamanho e a ordem dos elementos em um **contêiner** usando propriedades CSS.

O Flexbox é útil quando você deseja criar layouts complexos que se ajustam a diferentes tamanhos de tela. Ele é amplamente suportado pelos navegadores modernos e é fácil de usar com HTML e CSS.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1606910969576/3TzfJram_.png?auto=compress,format&format=webp)

## Cards
Cards são um elemento comum em layouts de páginas da Web. Eles são usados para**exibir informações em um formato compacto e fácil** de ler. Em CSS, você pode criar cards usando várias técnicas, como **CSS Grid e Flexbox**.

## Responsividade
Responsividade em HTML é uma técnica que permite que o conteúdo de um site se adapte a diferentes tamanhos de tela. Isso é importante porque as pessoas acessam sites em dispositivos com telas de diferentes tamanhos, como smartphones, tablets e computadores.
> :bulb: **Dica:** Para preparar a página à responsividade adicionar no `head` ` <meta name="viewport" content="width=device-width, initial-scale=1">`.


## O Exemplo
Este exemplo de flexbox é composto um uma pasta principal *flexbox* e dentro dela os seguintes elementos

- index.html (arquivo html)
- estilo.css (arquivo css)
- img (pasta de imagens)
   - R.png (imagem png)

### index.html
A estrutura da página está dividida em tres partes
- `<div class="cabecalho">` que contêm logo e titulo
- `<div class="container">` que contêm as cards
- `<div class="rodape">` que são as informações sobre autor e fonte.
Dentro da `div class="container"` tem a estrutura das cards, uma para cada personagem.

Cada ` <div class="card">` possui um titulo `h2` uma imagem `img` com algum link na internet e listas `ul` e parágrafos `p` para as informações sobre personagens.

> :bulb: **Dica:** Para adicionar mais uma card apenas copie e cole o codigo `<div class="card">...</div>`.

Para terminar tem `<div class="rodape">` com as informações sobre autor e a fonte.


## estilo.css
```css
body {
    font-family: Arial, sans-serif;
    color: #ffffff;
    background-image: url('https://cutewallpaper.org/21/naruto-akatsuki-wallpaper/Akatsuki-Wallpaper-iPhone-58-images.jpg');
    background-position: center;
    background-size: cover;
    background-attachment: fixed;
}
```
Aqui &uarr; estão configurados o fundo e a tipografia geral da página (tipo de fonte e cor). O fundo é fixado, centralizado e toma a largura toda da página. Usei uma imagem com tamanho de alta resolução

```css
h1{
    font-size: 50px;
    text-align: center;
    font-family:cursive, sans-serif;
    font-size: 48px;
    color: #ffcc00;
    text-shadow: 2px 5px #000000;
   }
```
Aquí  &uarr; temos o titulo, repare o `text-shadow: 2px 5px #000000;` para dar sombreamento.

```css
.logo{
       width: 20%; 
       display: block;
       margin: auto;
   }
```
A class .logo centraliza a imagem acima do titulo em sentido vertical.

> :warning: **Atenção:** O código a seguir serve para o flexbox.

```css
.container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    max-width: 1000px;
    margin: 0 auto;
    padding: 20px;
    font-family: Arial, Helvetica, sans-serif ;
    color:darkred;
  }
```
`display: flex; 
 flex-wrap: wrap;` permitem que a página adapte o conteúdo conforme flexbox, ou seja de esquerda para direita, e colocando em nova linha abaixo caso não tenha mais espaço.

`max-width: 1000px;
    margin: 0 auto;` servem para dar a largunra máxima ao container e contraliza-lo na página.

`justify-content: space-between;` serve para distribuir auomaticamente o espaço que sobrou entre as **cards**
```css
.card {
    background-color: #ffffff;
    border-radius: 5px;
    padding: 20px;
    width: 20%;
    margin-bottom: 20px;
  }  
  .card img {
    width: 100%;
    border-radius: 5px;
    margin-bottom: 10px;
  }
  
  .card h2 {
    font-size: 20px;
    margin-bottom: 10px;
    text-align: center;
  }
```    
 Este código fornece o estilo às cards, largura, texto, bordas, espaço das bordas, posicionamento e tamanho da imagem, etc. 

Para terminar

```css
 .rodape p
  {
    font-size:10px;
    text-align: center;
    font-family:cursive, sans-serif;
    color: #ffcc00;
    text-shadow: 2px 5px #000000;
  }

  .rodape a:hover
  {
    color: darkred;
  }

  .rodape a
  {
    color: #ffcc00;
  }
```
esta parte fornece o estilo básico para o rodapé das fontes com cores, tipos e tamanhos.

  



