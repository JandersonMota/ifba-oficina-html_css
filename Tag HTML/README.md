# Tags HTML

## O que é HTML?
Linguagem de Marcação de Hipertexto (HyperText Markup Language). Sua responsabilidade principal é demarcar a estrutura de uma página da web.

## O que é Tag?
São instruções que informam ao navegador como formatar o conteúdo de uma página da web.

## Estrutura básica
```
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>

</body>
</html>
```

### `<!DOCTYPE html>`
É uma instrução que indica ao navegador qual versão do HTML deve ser usada para exibir uma página. Sem essa declaração, os navegadores podem entrar no *`"quirks mode"`*, o que pode fazer com que a página seja exibida de maneira inesperada.

### `<html>`
É a raiz de um documento HTML. Ela define o início e o fim de todo o conteúdo HTML que será exibido na página da web.

### `<head>`
Contém informações dos metadados sobre a página, além de links para recursos externos como folhas de estilo (CSS), scripts (JavaScript) e outras instruções para o navegador.

### `<meta>`
Fornece informações sobre uma página web aos mecanismos de busca e navegadores. As meta tags são importantes para o SEO, ou seja, para o posicionamento do site nas páginas de resultados dos buscadores.

Pontos importantes do SEO:
- Facilitam o rastreamento da página pelo mecanismo de busca;
- Ajudam a organizar a página;
- Favorecem o posicionamento na SERP.

#### Funções comuns da tag `<meta>`:
**1. Especificar o conjunto de caracteres (charset):** Define qual conjunto de caracteres será utilizado na página (geralmente UTF-8, que suporta a maioria dos caracteres, incluindo letras acentuadas).
```
<meta charset="UTF-8">
```

**2. Descrição da página:** Fornece uma breve descrição da página, o que ajuda no SEO (otimização para motores de busca) e pode aparecer nos resultados de pesquisa.
```
<meta name="description" content="Esta é uma página de exemplo em HTML.">
```

**3. Palavras-chave (keywords):** Ajuda motores de busca a identificar o conteúdo da página, listando palavras-chave relevantes.
```
<meta name="keywords" content="HTML, exemplo, tutorial, metadados">
```

**4. Autor da página:** Informa o nome do autor ou responsável pela criação do conteúdo.
```
<meta name="author" content="Seu Nome">
```

**5. Controle de cache:** Indica ao navegador se ele deve armazenar ou atualizar o conteúdo da página. Por exemplo, para evitar o cache:
```
<meta http-equiv="cache-control" content="no-cache">
```

**6. Viewport (Importante para design responsivo):** Controla a forma como a página é exibida em dispositivos móveis, permitindo o ajuste do layout para telas menores.
```
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

**7. Redirecionamento e atualização automática:** Define um redirecionamento após um período de tempo específico. Por exemplo, para redirecionar após 5 segundos:
```
<meta http-equiv="refresh" content="5;url=https://www.exemplo.com">
```

#### Exemplo de uma seção <head> com várias tags <meta>:
```
<head>
    <meta charset="UTF-8">
    <meta name="description" content="Exemplo de uma página com metadados.">
    <meta name="keywords" content="HTML, meta tags, SEO">
    <meta name="author" content="Janderson Mota">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exemplo de Página</title>
</head>
```

### `<title>`
Define o título de uma página da web. Ela é importante para o SEO, pois ajuda os mecanismos de busca a entenderem o conteúdo da página e a classificar os resultados. Ela é um dos principais fatores que atraem visitantes ao site e pode ser a única oportunidade de chamar a atenção do leitor.

A tag `<title>` aparece em vários locais, como: Na aba do navegador, Na página de resultados de pesquisa (SERP), Nos posts de redes sociais.


**Nota:** SERP (Search Engine Results Page) é a página que os motores de busca, como o Google, Bing ou Yahoo, exibem após um usuário realizar uma pesquisa.

### `<body>`
É onde todo o conteúdo visível de uma página web é definido. Isso inclui textos, imagens, links, vídeos, botões, tabelas, formulários e outros elementos que os usuários podem interagir diretamente.

## Comparação de Tags Semânticas vs. Tags Não Semânticas

| **Tags Semânticas** | **Descrição**                                                 | **Tags Não Semânticas** | **Descrição**                        |
|----------------------|-------------------------------------------------------------|--------------------------|-------------------------------------|
| `<header>`           | Define o cabeçalho de uma seção ou página.                  | `<div>`                  | Um contêiner genérico sem significado específico.  |
| `<nav>`              | Define uma seção de navegação.                               | `<span>`                 | Um contêiner em linha sem significado específico.   |
| `<article>`          | Representa um conteúdo independente e auto-contido.         | `<b>`                    | Usado para enfatizar texto, mas sem significado semântico. |
| `<section>`          | Define uma seção do documento com um tema específico.       | `<font>`                 | Usado para alterar a aparência do texto, sem semântica. |
| `<footer>`           | Define o rodapé de uma seção ou página.                     | `<i>`                    | Usado para texto em itálico, sem significado semântico. |
| `<aside>`            | Define conteúdo relacionado, mas não essencial, à página.   | `<center>`               | Usado para centralizar texto, sem significado semântico. |
| `<figure>`           | Representa conteúdo ilustrativo, como imagens ou diagramas. | `<u>`                    | Usado para sublinhar texto, sem semântica.          |
| `<main>`             | Define o conteúdo principal do documento.                    | `<tr>`                   | Usado em tabelas, mas sem significado semântico por si só. |
| `<ol>`               | Define uma lista ordenada; a ordem dos itens é relevante.   |                          |                                     |
| `<ul>`               | Define uma lista não ordenada; a ordem dos itens não é relevante. |                          |                                     |
| `<li>`               | Define um item dentro de uma lista (`<ol>` ou `<ul>`).      |                          |                                     |

As **tags semânticas** ajudam os desenvolvedores e motores de busca a entender melhor a estrutura e o significado do conteúdo em uma página, enquanto as **tags não semânticas** são genéricas e não fornecem informações adicionais sobre o conteúdo que contêm.

Exemplo de estruturação com tags semânticas:

![image](https://github.com/user-attachments/assets/e1ff6368-e8ac-46cd-99a4-346846af284f)



## Tag `<main>`
Define o conteúdo principal de uma página web. O conteúdo dentro da tag `<main>` deve ser único e de maior relevância na página. Usar a tag `<main>` ajuda na acessibilidade e na estruturação semântica do documento, facilitando a navegação por leitores de tela e motores de busca.

> Fonte: <a href="https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/main">`<main>`</a>



## Tag `<section>`
É usado para agrupar conteúdo em blocos tematicamente relacionados dentro de uma página. Cada `<section>` deve ter um propósito claro e específico, com conteúdo que possa ser considerado independente ou destacado dentro do contexto da página. Ela é especialmente útil para estruturar documentos de maneira lógica e organizada.

> Fonte: <a href="https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/section">`<section>`</a>



## Títulos e Subtítulos
São usadas para organizar o conteúdo de um documento em diferentes níveis de importância ou hierarquia, de forma a estruturar bem as informações. Cada número indica um nível de hierarquia, onde `<h1>` é o título mais importante e `<h6>` é o menos importante.

| Tag         | Exemplo de Uso                     |
|-------------|-------------------------------------|
| `<h1>`      | `<h1>Título</h1>`                  |
| `<h2>`      | `<h2>Subtítulo</h2>`               |
| `<h3>`      | `<h3>Subtítulo</h3>`               |
| `<h4>`      | `<h4>Subtítulo</h4>`               |
| `<h5>`      | `<h5>Subtítulo</h5>`               |
| `<h6>`      | `<h6>Subtítulo</h6>`               |

`<h1>`: Representa o título principal da página ou do conteúdo. Recomendado ser usado uma única vez em um documento para representar o assunto principal.

`<h2>`: Usado para subtítulos principais que dividem o conteúdo em grandes seções ou categorias. São os tópicos principais dentro do título `<h1>`.

> Fonte: <a href="https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/Heading_Elements">`<h1>`-`<h6>`</a>



## Tag `<p>`
A tag `<p>` representa um parágrafo, que são usados para agrupar conteúdos relacionados de qualquer tipo, como imagens e campos de um formulário.

> Fonte: <a href="https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/p">`<p>`</a>



## Tag `<img>`
É usada para incorporar imagens em uma página web.

`<img src="" alt="" id="" class="" title="" loading="lazy">`

### Atributos Comuns da Tag `<img>`:
#### src (obrigatório)
- Define o caminho da imagem que deve ser exibida.
- Exemplo: `<img src="imagem.jpg">`

#### alt (obrigatório)
- Fornece uma descrição alternativa da imagem, que é exibida se a imagem não puder ser carregada. Também é importante para acessibilidade.
- Exemplo: `<img src="imagem.jpg" alt="Descrição da imagem">`

#### id
- Define um identificador único para a imagem.
- Exemplo: `<img src="imagem.jpg" id="minha-imagem">`

#### class
- Adiciona uma ou mais classes CSS à imagem para estilização.
- Exemplo: `<img src="imagem.jpg" class="minha-classe">`

#### title
- Fornece um texto que aparece como uma dica quando o mouse é passado sobre a imagem.
- Exemplo: `<img src="imagem.jpg" title="Título da imagem">`

#### loading
Controla o comportamento de carregamento da imagem. Os valores podem ser `lazy`, `eager` ou `auto`.

1. `loading="lazy"`
Utiliza o carregamento preguiçoso para otimizar a experiência do usuário em páginas web, adiando o carregamento de imagens até que sejam necessárias. Isso pode resultar em tempos de carregamento mais rápidos e menor uso de largura de banda.

- Carregamento Preguiçoso (Lazy Loading):
  - O atributo `loading="lazy"` informa ao navegador para adiar o carregamento da imagem até que ela esteja próxima da área visível (viewport) do usuário. Isso significa que as imagens que não estão imediatamente visíveis na tela não são carregadas até que o usuário role a página para vê-las.

- Melhora de Performance:   
  - O lazy loading pode resultar em uma melhoria significativa no desempenho da página, especialmente em páginas que contêm muitas imagens. Isso reduz o tempo de carregamento inicial e diminui a quantidade de dados transferidos, resultando em uma melhor experiência para o usuário.

- Eficiência de Recursos:
  - Essa técnica é especialmente útil em dispositivos móveis ou em conexões de internet mais lentas, onde o carregamento de todas as imagens de uma vez poderia levar muito tempo e consumir muitos dados.

#### Outros atributos mais comuns que podem ser usados com a tag `<img>`:
width, height, style, usemap, usemap, usemap e usemap.

> Fonte: <a href="https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/img">`<img>`</a>



## Tag `<form>`
A tag `<form>` é usada para criar um formulário interativo que coleta dados do usuário e os envia para um servidor. Ela serve como um contêiner para vários tipos de campos de entrada, como caixas de texto, botões de rádio, caixas de seleção, menus suspensos, e botões de envio. Os dados coletados por meio do formulário podem ser enviados para um servidor para processamento, como via uma requisição HTTP.

### Atributos que podem ser usados na tag `<form>`:

#### `action`
Define a URL para onde os dados do formulário serão enviados.

#### `method`
Especifica o método HTTP para enviar os dados. Os valores mais comuns são:
- `"GET"`: Os dados são anexados à URL na barra de endereços.
- `"POST"`: Os dados são enviados no corpo da requisição HTTP, sendo mais seguro e usado para enviar grandes quantidades de dados.

#### `enctype`
Define o tipo de codificação dos dados que serão enviados, importante para uploads de arquivos.
- `"application/x-www-form-urlencoded"`: Padrão para formulários simples.
- `"multipart/form-data"`: Usado quando o formulário contém upload de arquivos.

#### `target`
Especifica onde a resposta será exibida, como em uma nova aba ou janela.
- `_blank`: Abre a resposta em uma nova aba ou janela.

#### `autocomplete`
Especifica se o navegador pode ou não sugerir automaticamente os dados anteriormente inseridos.

> Fonte: <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form">`<form>`</a>



## Tag `<fieldset>`
A tag `<fieldset>` é usado para agrupar visual e semantemente campos relacionados dentro de um formulário. Ele ajuda a organizar os campos de forma lógica, facilitando a compreensão tanto para os usuários quanto para as tecnologias assistivas. Visualmente, o `<fieldset>` é exibido com uma borda em torno dos campos agrupados, o que ajuda a destacar que aqueles elementos pertencem a uma mesma categoria ou seção.

> Fonte: <a href="https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/fieldset">`<fieldset>`</a>



## Tag `<legend>`
A tag `<legend>` é frequentemente usada dentro de `<fieldset>` para fornecer uma legenda ou título para o grupo de campos, explicando o propósito do agrupamento.

> Fonte: <a href="https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/legend">`<legend>`</a>



## Tag `<label>`
é usada para associar uma descrição ou rótulo a um elemento de formulário, como um campo de entrada (`<input>`, `<select>`, `<textarea>`, etc.). O principal objetivo da tag `<label>` é melhorar a acessibilidade e a usabilidade de formulários em páginas web, e pode ser configurada com uma série de atributos. Ela garante que os formulários sejam mais fáceis de usar, tanto para usuários comuns quanto para aqueles que dependem de tecnologias assistivas.

### Atributos que podem ser usados na tag `<label>`:

#### for
- Associa o rótulo a um elemento de formulário específico, por meio do valor do atributo id do elemento. Quando o usuário clica no rótulo, o foco é transferido para o campo de formulário correspondente.
- Exemplo: `<label for="nome">Nome Completo</label> <input id="nome" type="text">`

#### id:
- Define um identificador único para o rótulo. Isso é útil para estilização ou para referências em scripts.
- Exemplo: `<label id="rotuloEmail" for="email">E-mail</label>`

#### class:
- Define uma ou mais classes CSS para estilizar o rótulo.
- Exemplo: `<label class="label-principal" for="email">E-mail</label>`

#### Outros atributos mais comuns que podem ser usados com a tag `<label>`:
`form`, `style`, `title`, `lang`, `dir`, `accesskey`, `hidden`, `aria-*`, `tabindex`.

> Fonte: <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label">`<label>`</a>



## Tag `<input>`
Ela é usada para criar campos interativos onde os usuários podem inserir dados, ou seja, é essencial para coletar dados de usuários em um formulário.

`<input type="" name="" id="" class="">`

### Atributos Comuns da Tag `<input>`:
- Define o tipo de campo de entrada. Pode ser um dos vários valores, como `text`, `password`, `email`, `number`, `checkbox`, `radio`, `file`, `submit`, entre outros.

#### type (obrigatório)
- Atribui um nome ao campo de entrada, que é usado ao enviar o formulário para identificar o dado.
- Exemplo: `<input type="text">`

#### name (obrigatório)
- Atribui um nome ao campo de entrada, que é usado ao enviar o formulário para identificar o dado.
- Exemplo: `<input type="text" name="username">`

#### id
- Define um identificador único para o campo, útil para scripts e estilos.
- Exemplo: `<input type="text" id="username">`

#### class
- Adiciona uma ou mais classes CSS à imagem para estilização.

#### value
- Define um valor inicial ou o valor atual do campo de entrada.
- Exemplo: `<input type="text" value="valor">`

#### placeholder
- Exibe um texto de sugestão dentro do campo até que o usuário insira algum valor.
- Exemplo: `<input type="text" placeholder="Digite seu nome">`

#### required
- Indica que o campo é obrigatório e o formulário não será enviado se ele estiver vazio.
- Exemplo: `<input type="text" required>`

#### disabled
- Desabilita o campo de entrada, tornando-o não interativo e excluindo-o da submissão do formulário.
- Exemplo: `<input type="text" disabled>`

#### maxlength:
- Define o número máximo de caracteres que podem ser inseridos no campo.
- Exemplo: `<input type="text" maxlength="10">`

#### minlength:
- Define o número mínimo de caracteres que devem ser inseridos no campo.
- Exemplo: `<input type="text" minlength="5">`

#### pattern:
- Define uma expressão regular (regex) que o valor de entrada deve corresponder.
- Exemplo: `<input type="text" pattern="[A-Za-z]{3,}">`

#### formmethod:
- Especifica o método HTTP (GET ou POST) para o envio dos dados do formulário.
- Exemplo: `<input type="submit" formmethod="post">`

#### inputmode:
- Especifica o tipo de teclado que deve aparecer em dispositivos móveis, como `decimal`, `numeric`, `email`.
- Exemplo: `<input type="text" inputmode="numeric">`

#### Outros atributos mais comuns que podem ser usados com a tag `<input>`:
`readonly`, `min` e `max`, `step`, `autofocus`, `autocomplete`, `multiple`, `size`, `form`, `list`, `accept`, `alt`, `src`, `height` e `width`, `formaction`, `formenctype`, `formnovalidate`, `formtarget`.

> Fonte: <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input">`<input>`</a>



## Tag `<footer>`
A tag `<footer>` é utilizada para definir o rodapé de uma seção ou de um documento. Ela geralmente contém informações relacionadas ao conteúdo que a precede, como direitos autorais, informações de contato, links de navegação, ou outras informações pertinentes.

> Fonte: <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/footer">`<footer>`</a>



## Atributos globais
Atributos globais são atributos comuns a todos os elementos HTML; eles podem ser usados em todos os elementos, embora possam não ter efeito em alguns elementos.

EX.: `class`, `id`, `hidden`, `style`, `title` e etc.

> Fonte: <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes">Atributos globais</a>
