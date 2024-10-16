# O que é Reset CSS?

Reset CSS é uma técnica utilizada para remover ou "zerar" os estilos padrão que os navegadores aplicam a elementos HTML. O objetivo é garantir que todos os navegadores renderizem os elementos de forma consistente, eliminando discrepâncias entre diferentes navegadores e suas interpretações de estilos.

## Por que usar Reset CSS?
**Consistência:** Diferentes navegadores têm estilos padrão variados para elementos como margens, preenchimentos, fontes, etc. O Reset CSS garante que você comece com uma base comum, tornando mais fácil estilizar sua página da maneira desejada.

**Simplificação:** Ao eliminar estilos padrão, o desenvolvedor pode ter um maior controle sobre o layout e a aparência dos elementos, evitando surpresas que podem surgir devido a estilos indesejados.

**Melhoria da Acessibilidade:** Um estilo mais uniforme pode ajudar a criar uma melhor experiência para todos os usuários, incluindo aqueles que utilizam tecnologias assistivas.

## Reset CSS
Compreendemos que para reduzirmos as formatações originais entre diferentes navegadores, precisamos selecionar todas as tags e adicionar sobre elas os resets, como margin, padding, border, etc.

Cada pessoa pode criar o seu próprio reset CSS a partir da necessidade do seu projeto ou pode também utilizar algum reset pronto.

Um dos mais utilizados e conhecidos foi desenvolvido pelo Eric Meyer. No [blog] (https://meyerweb.com/eric/tools/css/reset/), ele explica um pouco sobre a técnica e como desenvolveu o seu código reset.

``` reset.css
/* http://meyerweb.com/eric/tools/css/reset/ 
   v2.0 | 20110126
   License: none (public domain)
*/

html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed, 
figure, figcaption, footer, header, hgroup, 
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
	margin: 0;
	padding: 0;
	border: 0;
	font-size: 100%;
	font: inherit;
	vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article, aside, details, figcaption, figure, 
footer, header, hgroup, menu, nav, section {
	display: block;
}
body {
	line-height: 1;
}
ol, ul {
	list-style: none;
}
blockquote, q {
	quotes: none;
}
blockquote:before, blockquote:after,
q:before, q:after {
	content: '';
	content: none;
}
table {
	border-collapse: collapse;
	border-spacing: 0;
}
```
O mais habitual é que antes de se começar a estilizar o projeto, o arquivo reset CSS já seja adicionado para que seja feita a remoção da formatação original dos browsers.

Isso porque, caso o reset CSS seja adicionado no meio do projeto, por exemplo, pode gerar dores de cabeça já que o layout foi criado utilizando como referência a formatação dos navegadores e não na padronização dos elementos que foram resetados.
