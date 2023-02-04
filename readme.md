<h1 align="center"> Desafio Avançado - Recriando layout </h1>

<img src=".github\rocketsect.png">


## Tecnologias  

- HTML
- CSS
<br>

## Projeto

Desafio proposto pela escola Rocketseat para treino e fixação de conhecimento e técnicas de ```flexbox```.

Nele tomei liberdade de pequenas alterações.
Que foi no caso de adicionar um efeito ```hover``` de borda utilizando ```opacity``` e ```width``` no elemento ```background```. Com o pseudo-elemento ```after```. Que, ao passar o mouse sob o objeto ele "ativa" o pseudo-elemento com uma transição. criando um efeito de uma borda se expandindo. Que nada mais é que um fundo, fino e transparente que ganha opacidade e preenchimento.

O código usado para conseguir este efeito foi esse:
```css

a {
  color:#FFFFFF;
  text-decoration: none;    /* base */
  font-size: 14px;
  line-height: 28px;
}

a:after {
  content: "";
  display: flex;
  justify-content: center;
  width: 0;
  background: #6cb1a8;    /* borda que está "hibernando"*/
  height: 2px;
  opacity: 0;
  transition: opacity, width;
  transition-duration: .2s;
}

nav a:hover:after {
  opacity: 1;    /*preenchimento e opacidade que terão efeito com a transição*/
  width: 100%;
}
```



