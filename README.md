# easy.css

*Combine as classes para ter o melhor resultado em seus projetos*

`easy.css` é uma pequena biblioteca com os estilos mais usados pelos Desenvolvedores WEB, desta forma fica bem fácil criar um código limpo, bonito e legível.

## Instalação
   1. Inclua o 'stylesheet' no `<head>` do documento

```html
<head>
    <link rel="stylesheet" href="easy.css">
</head>
```
  
    2. Combine as classes desejadas ao elemento que desejar. Exemplo:
```html
 <h1 class="p-0 mb-40 inline-block">Exemplo</h1>
```
*Nota: Acima estamos declarando que o h1 tem padding 0, margin-bottom 40px e display inline-block*
    
    
## Conheça as Classes
Vamos detalhar Classe por Classe, mas fica mais fácil se pensar de forma lógica para as nomenclaturas quando estiver codificando.

*Vamos separar por 5 categorias: **Padding**, **Margin**, **Fonts**, **Hacks** e **Overlap**.*


### Padding

Na biblioteca os valores do `padding` são de 0 ate 400px com escala de multiplus de 5. Exemplo:

```note
.p-0
.p-5
.p-10
…
.p-200
.p-205
.p-210
...
.p-390
.p-395
.p-400
```

*Nota: usando a class p-* sera adicionado ao seu elemento padding nos 4 cantos*


##### Padding Left

É possível direcionar para onde deseja colocar o estilo, como por exemplo:

```html
<h1 class="pl-50">Exemplo Padding Left</h1>
```
*Nota: desta forma nosso elemento tem 50px de padding pra esquerda*

##### Padding Right, Top e Bottom

Acontece da mesma forma do exemplo do left, bastando apenas colocar a primeira letra da direção que deseja. Exemplp:

```html
<h1 class="pr-40 pt-60 pb-100">Exemplo Padding em diversas direções</h1>
```
*Nota: desta forma nosso elemento tem padding de 40px pra direita, 50px no topo e 100px na parte de baixo*


##### Padding com duas declarações de estilo

Para facilitar a vida também pode se usar a class `.ptb` (*padding top bottom*) para adicionar paddings iguais no topo e na parte inferior. Exemplo

```html
<h1 class="ptb-200">Exemplo PTB</h1>
```
*Nota: desta forma nosso elemento tem 200px de padding tanto no topo quanto na parte inferior*


Existe a possibilidade de declarar padding para esquerda e direita de uma só vez:

```html
<h1 class="plr-30">Exemplo PLR</h1>
```

### Margin

Declarar `margin` é tão simples quanto o `padding` e também usa o mesmo conceito de direções. 

Os valores do `margin` são de 0 ate 400px com escala de multiplus de 5, idêntico ao `padding`

```html
<h1 class="m-50">Exemplo Margin</h1>
```
*Nota: desta forma nosso elemento tera 50px de margin nos 4 cantos*



### Font

O `easy.css` facilita declarar o tamanho da font, espessura e distancia das linhas do seus textos.


#### Tamanho das fonts

Os valores do tamanho são de .01em a 13em. Exemplo:

```note
.s-dot1 = font-size: .1em
.s-dot2 = font-size: .2em
.s-dot3 = font-size: .3em
...
.s-1 = font-size: 1em
.s-1dot1 = font-size: 1.1em
.s-1dot2 = font-size: 1.2em
...
.s-12dot8 = font-size: 12.8em
.s-12dot9 = font-size: 12.9em
.s-13 = font-size: 13em

```

_Exemplo de uso:_

```html
<p class="s-1dot5">Exemplo</p>
```
*Nota: desta forma nosso elemento tem font-size de 1.5em*


#### Espessura

As espessuras são divididas em 6 tipos com 2 variações cada, são elas:

   **Extra Light** 
   * _.f-extra-light (font-weight:200;)_
   * _.f-extra-light-italic (font-weight:200; font-style:italic;)_
      

   **Light**
   * _.f-light (font-weight:300)_
   * _.f-light-italic (font-weight:300; font-style:italic;)_
   
   
   
   **Regular**
   * _.f-regular (font-weight:400;)_
   * _.f-regular-italic (font-weight:400; font-style:italic;)_
   
   
   
   **Semi Bold**
   * _.f-semi-bold (font-weight:600;)_
   * _.f-semi-bold-italic (font-weight:600; font-style:italic;)_
   
   
   
   **Bold**
   * _.f-bold (font-weight:700;)_
   * _.f-bold-italic (font-weight:700; font-style:italic;)_
         
   
   
   **Extra Bold**
   * _.f-extra-bold (font-weight:800;)_
   * _.f-extra-bold-italic (font-weight:800; font-style:italic;)_
    


_Exemplo:_
```html
<p class="f-bold-italic">Exemplo</p>
```
*Nota: desta forma nosso elemento seria bold e itálico*


#### Distancia entre as linhas

Os valores das distancias são de .01em a 13em. Exemplo:

```note
lh-dot1 = line-height: line-height: .1em;
lh-dot2 = line-height: line-height: .2em;
lh-dot3 = line-height: line-height: .3em;
...
lh-1 = line-height: line-height: 1em;
lh-1dot1 = line-height: line-height: 1.1em;
lh-1dot2 = line-height: line-height: 1.2em;
lh-1dot3 = line-height: line-height: 1.3em;
...
lh-12dot8 = line-height: line-height: 12.8em;
lh-12dot9 = line-height: line-height: 12.9em;
lh-13 = line-height: line-height: 13em;
```
_Exemplo:_

```html
<p class="lh-1dot4">Exemplo</p>
```
*Nota: desta forma nosso elemento tem um espaçamento entre as linhas de 1.4em*


### Hacks

As `hacks` são classes ja definidas, conheça:


**_.row-eq-height_**
Ele deixa as divs de dentro com a mesma altura
```css
.row-eq-height {
    display: -webkit-box;
    display: -webkit-flex;
    display: -ms-flexbox;
    display: flex;
}
```

**_.center-y_**
Centraliza o elemento no eixo Y
```css
.center-y {
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    width: 100%;
}
```

**_relative_**
Apenas define nosso elemento como relativo
```css
.relative{
    position: relative;
}
```

**_inline-block_**
Muda nosso elemento pra display inline-block
```css
.inline-block{
    display: inline-block !important;
}
```


**_break-word_**
Adicionar quebra de palavra
```css
.break-word{
    word-wrap: break-word;
}
```


**_hover-underline_**
Link com underline no hover
```css
.hover-underline{
    text-decoration: none;
}
.hover-underline:hover{
    text-decoration: underline !important;
}
```


**_no-underline_**
Link sem underline sempre
```css
.no-underline{
    text-decoration: none !important;
}
.no-underline:hover{
    text-decoration: none !important;
}
```


**_button-reset_**
Remove o background e a borda
```css
.button-reset{
    background: transparent;
    border: none;
}
```



**_btn-full_**
O link cobre toda a area do seu relative
```css
.btn-full{
    display: block;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    text-indent: -999999px;
    z-index: 10;
}
```



**_bg-cover_**
O bg preenche todo o elemento
```css
.bg-cover{
    -webkit-background-size: cover;
    background-size: cover;
}
```

**_Opacity_**
É bem simples, a transparência é dividida em uma escala de 1 a 10: ( _sendo 1 mais claro e 10 mais escuro_ )

```note
.opacity-1
.opacity-2
.opacity-3
.opacity-4
.opacity-5
.opacity-6
.opacity-7
.opacity-8
.opacity-9
.opacity-10
```




**_Placeholder Color_**
Quem trabalha com placeholder nos inputs sabe o quanto eles são chatos de trocar as cores, no `easy.css` ja temos 2 cores definidas, preto e branco.

```note
.place-black
.place-white
```


**_Border Radius_**
Pra deixar a borda arredondada usamos um escala de 0 a 100 com intervalo de 5 em 5 porcento.

```note
.radius-0
.radius-5
.radius-10
...
.radius-50
.radius-55
.radius-60
...
.radius-90
.radius-95
.radius-100
```