##### Hypertext Markup Language
<h1 id="inicio">Elementos</h1>

Os elementos são a totalidade do que engloba a tag, incluindo ela.
Uma das características mais interessantes em questão de praticidade e organização é a semântica, mas o que ela representa?

<h5><small>
Escolha abaixo o coneito que gostaria de ler:<br>
<a href="#semantica"> Semântica </a> - <a href="#titulos"> Títulos e Parágrafos </a> - <a href="#listas"> Listas </a> - <a href="#citacoes"> Citações</a> - <a href="#abreviacao"> Abreviação </a> - <a href="#contato">Detalhes de Contato</a> <br> <a href="#descricao">Linha de Descrição</a> - <a href="#codigo">Representação de Código</a> - <a href="#elementos-gerais">Elementos gráficos</a></small></h5>

<h2 id="semantica">Semântica</h2>

É a organização e boa prática de criar class's, id's , data-*'s para que o trabalho de personalização visual e de programação seja feito com mais coerência e facilidade.

Você vai criar classes com grupos de dados que compartilhem significado e desse modo poderá configurá-los mais rapidamente ao utilizar a classe atribuida a eles.

Já a utilização dos ID's serve para poder personalizar e acessar mais facilmente conteúdos específicos da página, já que os Id's devem ser sempre exclusivos para um elemento, não se repetindo em outros.
<a href=#inicio>Voltar ao Início</a>

<h2 id="titulos">Títulos e Parágrafos</h2>

São uma maneira de organizar e hierarquizar a importância dos conteúdos apresentados no site.

As tags de título são <code> &lt;h1&gt;&lt;&frasl;h1&gt;, &lt;h2&gt;, &lt;h3&gt;, &lt;h4&gt;, &lt;h5&gt; e &lt;h6&gt;</code>, quanto maior o número, menor é o tamanho final da fonte. Desse modo podemos criar uma hierarquia baseada em tamanho para mostrar qual é o título mais importante, e quais são os sequentes.

A tag para parágrafos é a <code>&lt;p&gt; &lt;&frasl;p&gt;</code>, ela causa a quebra do conteúdo que está dentro dela, separando-o dos textos anteriores e posteriores, formando um parágrafo. Vale lembra que para fazer uma quebra de linha em algum momento a tag mais indicada é a <code>&lt;br&gt;</code>. Obs.: A tag de quebra de linhas pode ser utilizada de três maneiras (<code>&lt;br&gt; &lt;&frasl;br&gt; &lt;br&frasl;&gt;</code>)sem problemas, mas isso é uma exceção.

<a href=#inicio>Voltar ao Início</a>


<h2 id="listas">Listas</h2>

São muito úteis e fáceis de implementar.
cada linha da lista é envolta pela tag <code>&lt;li&gt;&nbsp;&lt;&frasl;li&gt;</code>. Essa tag deve ser repetida em todas as linhas de itens da lista.
Essa primeira lista deve ser colocada como filha de uma entre duas opções de tag de listas: <code>&lt;ul&gt;</code> ou <code>&lt;ol&gt;</code> outra tag.

A tag ul representa uma lista não ordenada, e é representada por pontinhos:

- ex1
- ex2
- ex3

Já a tag ol representa a lista ordenada:

1. ex1
4. ex2
5. ex3

<a href=#inicio>Voltar ao Início</a>


<h2 id="citacoes">Citações</h2>

Existem três tags para criar citações no HTML:
1. <code>&lt;blockquote&gt;&nbsp;&lt;&frasl;blockquote&gt;</code> : é uma citação mais destacada usada para trechos de texto mais longos. Pode levar o atributo cite com o link para a fonte da citação, mas não causa retorno algum, ou o elemento <code>&lt;cite&gt;</code> que serviria para citar o nome do autor da citação.;
2. <code>&lt;cite&gt;&nbsp;&lt;&frasl;cite&gt;</code> : é uma citação que dá um pequeno destaque ao texto citado. É mais indicada pra citar a autoria da citação, de uma peça, obra de arte, etc. 
3. <code>&lt;q&gt;&nbsp;&lt;&frasl;q&gt;</code> : destaca entre aspas duplas o trecho que a integra como conteúdo.

<a href=#inicio>Voltar ao Início</a>


<h2 id="abreviacao">Abreviação</h2>

Ao ser utilizada esta tag, através do descanso do mouse sobre seu conteúdo, mostra o significado de uma abreviação. Sua sintaxe é a <code>&lt;abbr&gt;&nbsp;&lt;&frasl;abbr&gt;</code> e o atributo para a inclusão do significado da abreviação é o atributo title.

<a href=#inicio>Voltar ao Início</a>


<h2 id="contato">Detalhes de Contato</h2>


Como o próprio nome já diz, essa tag destaca os contatos do autor da página, não deve ser utilizada para qualquer tipo de contato ou endereço, senão os contatos do autor do HTML. Sua sintaxe é a <code>&lt;address&gt;&nbsp;&lt;&frasl;address&gt;</code>.

<a href=#inicio>Voltar ao Início</a>


<h2 id="descricao">Linha de Descrição</h2>


Tem a finalidade de criar um glossário, ou lista de palavras e seus significados. 
Sitaxe/exemplo:
<pre><code>
&lt;dl&gt;
    &lt;dt&gt;&nbsp;Alegria&nbsp;&lt;&minus;&minus;&excl;&nbsp;aqui entra o primeiro termo da lista a ser explicado&nbsp;&minus;&minus;&gt;&nbsp;&lt;&frasl;dt&gt;
    &lt;dd&gt;&nbsp;É a sensação de ser feliz.&nbsp;&lt;&minus;&minus;&excl;&nbsp;aqui entra a explicação&minus;&minus;&gt;&nbsp;&lt;&frasl;dd&gt;
    <br>
    &lt;dt&gt;&nbsp;Tristeza&nbsp;&lt;&minus;&minus;&excl;&nbsp;aqui entra o segundo termo a ser explicado&nbsp;&minus;&minus;&gt;&nbsp;&lt;&frasl;dt&gt;
    &lt;dd&gt;&nbsp;É a ausência de alegria.&nbsp;&lt;&minus;&minus;&excl;&nbsp;aqui entra a explicação&nbsp;&lt;&frasl;dd&gt;
&lt;&frasl;dl&gt;
</code></pre>

Resultado do exemplo acima:

<dl>
    <dt>Alegria</dt>
    <dd>É a sensação de ser feliz.</dd>
    <dt>Tristeza</dt>
    <dd>É a ausência de alegria.</dd>
</dl>

<a href=#inicio>Voltar ao Início</a>


<h2 id="codigo">Representação de Código</h2>

É uma tag para que seja possível mostrar um código, por escrito, na página, como um exemplo, sem executar o mesmo.

Sintaxe:
<code>&lt;code&gt;&nbsp;&lt;&frasl;code&gt;</code> é utilizado para mostrar códigos curtos de uma linha, para mostrar códigos maiores e respeitando indentações, utiliza-se o <code>&lt;pre&gt;&nbsp;&lt;&frasl;pre&gt;</code> ao redor do <code>&lt;code&gt;&nbsp;&lt;&frasl;code&gt;</code> como no exemplo a seguir: <pre><code>&lt;pre&gt;&lt;code&gt;&nbsp;
Aqui entra o código
&lt;&frasl;code&gt;&lt;&frasl;pre&gt;</code></pre>

<a href=#inicio>Voltar ao Início</a>


<h2 id="elementos-gerais">Elementos Gerais</h2>

São o <code>&lt;div&gt;&nbsp;&lt;&frasl;div&gt;</code> e o <code>&lt;span&gt;&nbsp;&lt;&frasl;span&gt;</code>.

O div serve para separar elementos em diferentes blocos, é muito útil para a organização e layout da página, a fim de agrupar elementos e separar elementos entre si. Está quase sempre associado a um um atributo class, já que deste modo fica mais fácil selecionar o que leva as características de uma classe e o que não leva.

O span tem a mesma utilidade, mas diferente do div, não separa num novo bloco, mantém os elementos em linha.

<a href=#inicio>Voltar ao Início</a>


