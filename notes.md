## Web Semântica

Veremos a importância de se ter um HTML5 semântico, suas tags e um conjunto de elementos semânticos mais utilizados na Web.

Web Semântica significa adicionar significado a uma linguagem. No caso do HTML, é para dar significado ao conteúdo, facilitando a visualização e manutenção da estrutura montada.

A Web Semântica controla a organização e a apresentação do conteúdo. Mas, apesar de cada site ser único, existem padrões/convenções que podem ser identificados intencionalmente ou não.

Ao utilizar uma marcação semântica consistente, para identificar os elementos da página, ajudamos os `user agents` (navegador) a identificar corretamente os elementos e apresentá-los aos visitantes da página.

Isso faz com que a acessibilidade tenha destaque e visitantes com necessidades especiais possam fazer bom uso da página.

Além de ajudar na parte de acessibilidade, os motores de busca dão preferência para sites que estão com sua semântica bem estruturada e organizada.

### Importância das tags HTML5

A tags irão ajudar a criar um HTML semântico, pois algumas tags têm significados específicos e orientações claras sobre onde devem ficar na página e o motivo dela existir.

Exemplo:

```html
<p>Todo ponto de vista é a vista de um ponto. - Leonardo Boff</p>
```

Melhor semântica:

```html
<blockquote>
  Todo ponto de vista é a vista de um ponto.
  <cite>- Leonardo Boff</cite>
</blockquote>
```

Dessa forma, ao abrir a estrutura da página para pesquisar onde está tal citação, será encontrada com muito mais facilidade, fora as vantagens de ter o HTML mais semântico (auxílio no CSS e JavaScript, acessibilidade, SEO...).

#### Nas é possível fazer tudo só com `<p>`?

Sim, mas o foco do HTML5 é melhorar a semântica. E conforme for estudando, tentar ao máximo buscar refras e padrões para aprimorar a estrutura do documento.

### Seções comuns

São elas:

- cabeçalho `<header>`;
- navegação `<nav>`;
- conteúdo principal `<main>`;
- barra lateral `<aside>`;
- rodapé `<footer>`.

#### Header

Elemento estrutural e semântico, o header não possui atributos específicos.

É, geralmente, utilizado no início da página, sendo assim visto como global.

Pode ser usar também em outros elementos semânticos, como article e section. Não faz sentido usar header dentro de header e header dentro de footer, pois perde-se a semântica dele.

#### Nav

Não possuem atributos específicos, só globais.

Serve para representar uma seção da página que vai apontar para outras páginas ou áreas da nossa página.

Geralmente, vêm dentro do header, sendo a nav principal. Mas é importante saber que nem todos os links da página devem estar dentro da tag nav, que é mais destinada para links importantes.

Por exemplo, no "sitemap", geralmente alocado ao footer, não é preciso inserir os links dentro da Nav.

A nav sempre vai representar algo muito especial do site, então é importante saber onde utilizá-la.

Leitores de tela usam o nav para tomar decisões na página.

#### Main

Não possuem atributos específicos, só globais.

Tag para conteúdo único da página, aplicado diretamente dentro do body, uma vez por página.

Entedemos que conteúdo principal aquele que é relacionado diretamente com o tópico central da página ou com a funcionalidade central de sua aplicação.

Dentro de main, não é colocado, por exemplo: blocos de publicidade e menu.

```html
<body>
  <main>
    <h1>Sucos Detox</h1>
    <p>Página de sucos Detox</p>

    <article>
      <h2>Suco de Abacaxi com Gengibre</h2>
      <p>Muito fácil de fazer esse suco detox de abacaxi com gengibre.</p>
    </article>

    <article>
      <h2>Suco de Maçã com Côco</h2>
      <p>Muito fácil de fazer esse suco detox de maçã com côco.</p>
    </article>
  </main>
</body>
```

#### Article

Não possuem atributos específicos, só globais.

Como visto acima, o article vai construir um bloco de conteúdo que são relacionados.

Podem se repetir pela página e representam uma composição independente do documento.

#### Aside

Ajuda a descrever conteúdos levemente relacionados ao conteúdo principal.

Por exemplo:

- explicações;
- glossários;
- links extras;
- biografia do autor;
- informações de perfil.

Aside não tem a ver com o sidebar.

#### Footer

Geralmente, fica no final da página e possui:

- informações do autor;
- copyright;
- contato;
- sitemap;
- voltar ao topo.

Seus atributos são globais.

#### Section

Serve para colocar seções na página e, geralmente, a boa prática é que a section possua um título.

Alguns exemplos:

```html
<section>
  <h2>Contato</h2>
  <p>Fale conosco.</p>
</section>
```

```html
<article>
  <h2>Receita 1</h2>
  <p>Confira como fazer a receita.</p>

  <section>
    <h3>Modo de preparo</h3>
    <p>Descrevendo o modo de preparo.</p>
  </section>
</article>
```

```html
<main>
  <h1>Receita 1</h1>
  <p>Confira como fazer a receita.</p>

  <section>
    <h2>Modo de preparo</h2>
    <p>Descrevendo o modo de preparo.</p>
  </section>
</main>
```

Antigamente, usava-se `div` para fazer uma seção, mas, semanticamente, é melhor utilizar a tag `section`.

### Elementos genéricos não-semânticos

Escrever HTML semântico é um processo que leva tempo. Temos dois elementos que se aplicam para uso genérico, enquanto não conseguimos encontrar elementos semânticos para texto e/ou bloco.

Em ambas as situações, usam-se atributos globais, como `id` e `class`, para entregar maior significado.

`<div></div>`: usado se não conseguir achar elemento de bloco semântico. <br><br>
A ideia da section, por exemplo, é ter um contexto relacionado à página e não um contexto global do site inteiro. Um carrinho de compras, por exemplo, tem um contexto global, do site inteiro, e não somente a uma página. Nesse caso, aplicaríamos uma `div` com uma classe.<br>

```html
<div class="cart">
  <h2>Carrinho de compras</h2>
</div>
```

Mas temos que ter atenção com a `div` para não usá-la em excesso, para que possamos deixar o HTML semântico.

`<span></span>`: usado se não conseguir achar elemento de texto semântico. Substitui alguma marcação em um texto. <br>

```html
<h1>Título <span class="destaque">destacado</span></h1>
```
