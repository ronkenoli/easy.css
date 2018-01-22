# easy.css

*Combine as classes para ter o melhor resultado em seus projetos*

`easy.css` é uma pequena biblioteca com os estilos mais usados pelos desenvolvedores WEB, desta forma fica bem fácil criar um código limpo e bonito e legível.

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
Vamos detalhar Classe por Classe, mas vai ajudar se pensar de forma logica as nomeclaturas quando estiver codificando.

*Vamos separar por 5 categorias: Padding, Margin, Fonts, Hacks e Overlap.*


### Padding

Na biblioteca os valores do `padding` são de 0 ate 400px com escala de multiplos de 5. Exemplo:

```note
.p-0 = padding: 0;
.p-5 = padding: 5px;
.p-10 = padding: 10px;
.p-15 = padding: 15px;
...
.p-390 = padding: 390px;
.p-395 = padding: 395px;
.p-400 = padding: 400px;
```

*Nota: usando a class p- sera adicionado ao seu elemento padding no 4 cantos*


##### Padding Left

É possivel direcionar para onde deseja colocar o estilo, como por exemplo:

```html
<h1 class="pl-50">Exemplo Padding Left</h1>
```
*Nota: desta forma nosso elemento tem 50px de padding pra esquerda*

##### Padding Right, Top e Bottom

Acontece da mesma forma do exemplo do left, bastando apenas colocar a primera letra da direção que deseja:

```html
<h1 class="pr-40 pt-60 pb-100">Exemplo Padding em diversas direções</h1>
```

*Nota: desta forma nosso elemento tem 40px de padding pra direita, 50px no topo e 100px na parte de baixo*


##### Padding com duas declarações de estilo

Para facilitar a vida também pode se usar a class `.ptb` (*padding top bottom*) para adicionar paddings iguais no topo e na parte inferior. Exemplo


```html
<h1 class="ptb-200">Exemplo PTB</h1>
```

*Nota: desta forma nosso elemento tem 200px de padding tanto no topo quanto na parte inferior*


Também existe a possibilidade de declarar paddin para esquerda e direita de uma só vez:

```html
<h1 class="plr-30">Exemplo PLR</h1>
```

### Margin

Declarar `margin` é tão simples quanto o `padding` e também usa o mesmo conceito de direções. 

Os valores do `margin` são de 0 ate 400px com escala de multiplos de 5, identico ao `padding`


```html
<h1 class="m-50">Exemplo Margin</h1>
```

*Nota: desta forma nosso elemento tera 50px de margin em todos os cantos*



### Font

Com o `easy.css` fica fácil declarar o tamanho da font, espessura e distancia das linhas do seus textos.


##### Tamanho das fonts

Os valores do tamanho são de .01em a 13em. Exemplo:

```note
.s-dot1 = font-size: .1em
.s-dot2 = font-size: .2em
.s-dot3 = font-size: .3em
...
.s-1 = font-size: 1em
.s-1dot1 = font-size: 1.1em
.s-1dot2 = font-size: 1.2em
.s-1dot3 = font-size: 1.3em
...
.s-12dot8 = font-size: 12.8em
.s-12dot9 = font-size: 12.9em
.s-13 = font-size: 13em

```

######Exemplo:

```html
<p class="s-1dot5">Exemplo</p>
```

*Nota: desta forma nosso elemento tem 1.5em do tamanho da font*


##### Espessura

As espessuras são divididas em 6 com 2 variações cada, são elas:
     
   * .f-extra-light (font-weight:200;)
   * .f-extra-light-italic (font-weight:200; font-style:italic;)
   
   
   * .f-light (font-weight:300)
   * .f-light-italic (font-weight:300; font-style:italic;)
   
   
   * .f-regular (font-weight:400;)
   * .f-regular-italic (font-weight:400; font-style:italic;)
   
   
   * .f-semi-bold (font-weight:600;)
   * .f-semi-bold-italic (font-weight:600; font-style:italic;)
   
   
   * .f-bold (font-weight:700;)
   * .f-bold-italic (font-weight:700; font-style:italic;)
         
   
   * .f-extra-bold (font-weight:800;)
   * .f-extra-bold-italic (font-weight:800; font-style:italic;)
    

######Exemplo:

```html
<p class="f-bold-italic">Exemplo</p>
```

*Nota: desta forma nosso elemento seria bold italico*


##### Distancia entre as linhas

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

######Exemplo:

```html
<p class="lh-1dot4">Exemplo</p>
```

*Nota: desta forma nosso elemento tem um espaçamento entre as linhas de 1.4em*



















