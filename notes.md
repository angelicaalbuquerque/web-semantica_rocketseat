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

#### Main

#### Article

#### Aside

#### Footer

#### Section

### Elementos genéricos não-semânticos

```html

```
