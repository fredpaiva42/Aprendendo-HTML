# Aprendendo HTML

### Tags de Título

Os elementos em HTML têm tags de abertura como `<h1>`, e tags de fechamento, como `</h1>`.

Os elementos de título, que vão de **h1** a **h6**, são usados para dar significado à importância do conteúdo abaixo deles. Quanto menor o número, maior a importância. 

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