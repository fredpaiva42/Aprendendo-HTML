# Aprendendo HTML

### Tags de Título

Os elementos em HTML têm tags de abertura como `<h1>`, e tags de fechamento, como `</h1>`.

Os elementos de título, que vão de **h1** a **h6**, são usados para dar significado à importância do conteúdo abaixo deles. Quanto menor o número, maior a importância. 

Quando adicionamos um elemento de título menor à página, é implícito que estamos iniciando uma nova **subseção**.

>**Note**: Sempre usar apenas um elemento **h1** por página e colocar sempre os títulos de importância inferior abaixo dos mais importantes.

### Tag de Parágrafo

O elemento **p** é usado para criar um parágrafo de texto.


### Comentários em HTML

Comentários permitem que se possa deixar mensagens sem que elas apareçam na exibição do navegador. Também permite deixar códigos inativos. Um comentário em HTML é iniciado com `<!--` e finalizado com `-->`.

```HTML
<!--
    Este é um exemplo de comentário em HTML.
-->
```

### Tags Semânticas

O HTML5 tem alguns elementos que identificam diferentes áreas de conteúdo. Esses elementos tornam o HTML mais legível e ajudam com a otimização dos mecanismos de busca **(SEO)** e com a assebilidade. Alguns exemplos de tags desse tipo são as tags `<main>`, `<footer>`,`section`, etc.

### Aninhamento

Um elemento aninhado é "filho" de seu elemento "pai", ou seja, ele está contido no elemento "pai". Ele deve ser identado dois espaços a mais do que o elemento pai para melhorar a legibilidade, assim:

```HTML
<main>
    <p> Elemento filho </p>
</main>    
```

### Tag img e seus atributos

É possível adicionar imagens a um site usando o elemento **img**. Elementos **img** possuem tag de abertura, mas não de fechamento. Tags de elementos que não precisam de fechamento são conhecidas como *tags de fechamento automático*.

**Atributos** em HTML são palavras especiais usadas dentro da tag de abertura de um elemento para controlar o comportamento dele. Por exemplo, o atributo **src** em um elemento **img** especifica o caminho ou a URL da imagem que será usada.

Todos os elementos **img** devem ter um atributo **alt**. O texto de um atributo **alt** é usado por leitores de tela para melhorar a acessibilidade. Ele é exibido se a imagem não puder ser carregada.

### Uso de links

É possível linkar uma página a outra fazendo o uso do elemento âncora (**a**). Por exemplo:

```HTML
<a href="[http://](https://github.com/fredpaiva42)">Meu perfil no Github</a> <!-- Estou fazendo link para o meu perfil no github -->
```
O elemento âncora **a**, também tem atributos, como o **href** que faz referência a URL do site que deve ser redirecionado quando o usuário clicar no link.

O texto de um link dever ser colocado entre as tags de abertura e fechamento de um elemento âncora (**a**).

O elemento âncora **a** possui também um atributo chamado **target**, com ele é possível controlar se o link ao ser clicado pelo usuário irá ser aberto a uma nova gia ou não. Para que seja aberto em uma nova guia, é necessário usar o valor **_blank** no atributo **target**.

### Listas não ordenadas

A tag para a criação de uma lista não ordenada é a `<ul>` e para seus elementos da lista é a `<li>`:
```HTML
<ul>
    <li>milk</li>
    <li>cheese</li>
</ul>
```

### Listas ordenadas

Para uma lista ordenada a tag é `<ol>`.
```HTML
<ol>
    <li>milk</li>
    <li>cheese</li>
</ol>
```
### Figure

O elemento `<figure>` representa um conteúdo auto-contido e permite que se associe uma imagem com uma legenda.

O elemento de legenda da figura é adicionado pelo `<figcaption>` usado para descrever a imagem contida dentro do elemento.

### em

Para enfatizar deixando-o em itálico um texto no html podemos fazer o uso da tag `em`:
```HTML
Eu <em>amo</em> pizza <!--Dessa forma a palvra amo fica enfatizada-->
```

### strong

O elemento `<strong>` assim como o `em` enfatiza o texto, só que o strong deixa o texto em negrito.

### Formulários

Para criar um formulário em HTML devemos usar a tag `<form>`. A tag possui como um dos seus atributos o `action` que indica para onde os dados do formulário devem ser enviados.

Exemplo:
```HTML
<form action="/submit-url"></form>
<!--Nesse caso o action informa ao navegador que os dados do formulário devem ser enviados para o caminho /submit-url-->
```

### Input

É o elemento que nos permite varias maneiras de coletar dados a partir de um formulário web. Assim como o img é uma tag de fechamento automático.

O atributo `type` nos permite especificar qual é o tipo de entrada que queremos no nosso formulário, por exemplo, com o valor **text**, estamos definindo que o input vai receber dados do tipo texto.

Para que os dados de um formulário sejam acessados pelo local especificado no atributo `action`, é preciso dar ao campo de texto um atributo `name` e atribuir a ele um valor que represente os dados estão sendo enviados.
```HTML
<input type="text" name="email">
```

Outro atributo útil do input é o `placeholder`, nele podemos adicionar um valor que vai servir de exemplo de que tipo de dados devem ser inseridos naquele campo.

Temos também o `required` que ao ser adicionada faz com que só seja possível enviar o formulário se todos os campos tiverem sido preenchidos.

### Button

A tag `<button>` nos permite criar um botão. Para definir o texto do botão basta coloca-lo entre a tag de abertura e fechamento do button.
```HTML
<button>Esse é o texto que vai ser exibido no botão.</button>
``` 
O `button` envia por padrão para o endereço especificado no action do `form`, mas para que sempre fique claro é bom ter o costume de adicionar um atributo `type`, o atributo para enviar é o **submit**.

Para apresentar um botão com opção para perguntas onde o usuário deve dar apenas uma resposta entre várias opções. Basta adicionar um input com o `type` de valor **radio** e em seguida o nome da opção.
```HTML
<input type="radio"> SIM
```
Os elementos `label` são usados para ajudar a associar o texto de um elemento `input` com o próprio elemento (especialmente para tecnologias assistivas como leitores de tela.)
```HTML
<label><input type="radio">SIM</label>
```
isso torna possível que ao clicar na palavra **SIM** também selcione o botão de opção correspondente.

Para fazer com que ao selecionar um botão de opção automaticamente desmarque a seleção do outro, os dois botões precisam ter um atributo `name` com o **mesmo** valor.

 Os dados de formulário para botões são baseados em seus atributos **name** e **value**.

 A tag `fieldset` é usado para agrupar entradas (inputs) e rótulos (labels) relacionados em um formulário da web. Os elementos `fieldset` são *elementos de nível de bloco*, o que significa que eles aparecem em uma nova linha.

O elemento `legend` atua como uma legenda para o conteúdo do `fieldset`. Ele dá aos usuários contexto sobre o que devem inserir nessa parte do formulário.

Para perguntas que tenham mais de uma resposta usamos caixas de seleção, para ter uma entrada do tipo, basta que no atributo `type` do `input` seja inserido o valor **checkbox**.

### ID

O atributo `id` é usado para identificar elementos HTML específicos. O valor de cada atributo `id` deve ser **único** em comparação aos outros valores de `id` para a página inteira.