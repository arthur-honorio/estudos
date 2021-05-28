##### Hypertext Markup Language
<h1 id="inicio"> Conceitos </h1>

Como o próprio nome diz é uma linguagem que trabalha com marcações. Essas marcações fazem alterações no texto, disponibilizando capacidades que um texto comum não tem. 

O hipertexto é uma referência à possibilidade de utilização de mídias e comunicação com outros textos a partir desse primeiro.

<h5><small>
Escolha abaixo o coneito que gostaria de ler:<br>
<a href="#comentarios"> Comentários </a> - <a href="#tags"> Tags </a> - <a href="#atributos"> Atributos </a> - <a href="#atributos-globais"> Atributos Globais </a> - <a href="#aninhamento"> Aninhamento </a></small></h5>

<h3 id="comentarios">Comentários</h3>

Assim como as linguagens de programação, o HTML possui uma maneira de ter comentários e observações inseridos no corpo do texto sem que ele participe da configuração da página.

A utilidade é a de relembrar o programador do que foi feito, ou deixar claro para outro programadores o que precisa ser feito ali.

A sintaxe de comentário é a <code> &lt;&minus;&minus;&excl; O comentário entra aqui &minus;&minus;&gt; </code>.

<a href="#inicio"> Voltar par o Início </a>

<h3 id="tags"> Tags </h2>

Os tags são necessários para a abertura e o fechamento dos elementos HTML. Eles envolvem o conteúdo a ser formatado. Sua abertura acontece entre os sinais de menor (<) e maior (>) e seu fechamento é feito com a repetição da abertura adicionada de uma barra (/) antes do nome da tag. Ex.: <code>&lt;p&gt;  &lt;&frasl;p&gt;</code>.

Existem tags que não precisam de fechamento, elas são conhecidas como elementos vazios, e um exemplo é a tag <code>&lt;img&gt;</code> que não possui fechamento, seus atributos são inseridos dentro da própria abertura da tag. Ex.: <code>&lt;img src=&quot;&quot; alt=&quot;&quot;&gt;</code>.

Existem diversas tags e cada um tem uma função específica.

A tag <code>&lt;h1&gt;</code>, por exemplo, serve para criar títulos, o texto envolvido por ela ficará maior e numa versão bold.
A tag <code>&lt;html&gt;</code> inicializa a formatação de um texto HTML, ela deve aparecer no começo e no final do arquivo.

<a href="#inicio"> Voltar par o Início </a>


<h3 id="atributos">Atributos</h3>

Os atributos são infromações adicionais dadas aos elementos afim de conceder a eles características específicas e às vezes obrigatórias para o funcionamento correto do mesmo.

Um bom exemplo de atributos é o da tag "img": <code>&lt;img src=&quot;&quot; alt=&quot;&quot;&gt;</code>. A tag "img" tem como atributo obrigatório o "src" que informa a url onde será encontrada a imagem a ser exibida.

<a href="#inicio"> Voltar par o Início </a>


<h3 id="atributos-globais">Atributos globais</h3>

São atributos que podem ser utilizados em qualquer tag, mesmo que não tenham função para algumas, não gerará um problema.

Os mais comuns são: 
- *class:* atribui um classe ao elemento que a possui. São utilizados para classificar elementos em grupos que receberão mesmo tratamento em futuras utilizações;
- *id:* atribui un identificador exclusivo ao elemento que o recebe. São utilizados para aplicar configurações específicas por Id.;
- *title:* recebe um texto alternativo que será exibido por alguns navegadores quando o ponteiro do mouse ficar alguns segundos parado sobre o elemento.
- *data-\*:* atribui ao elemento um novo valor para classificação específica.
- *contenteditable:* dão ao usuário a possibilidade de editar o conteúdo deste elemento.
- *tabindex:* atribuem ao elemento que o recebe um lugar numa sequência de deslocamentos do cursor ao se apertar a tecla tab do teclado para navegação sem mouse.

<a href="#inicio"> Voltar par o Início </a>


<h3 id="aninhamento"> Aninhamento e Hierarquia </h3>

O aninhamento nada mais é do que a possibilidade de utilizar tags dentro de tags. Ao se fazer isso é adicionada uma hierarquia à estrutura, sendo os tags internos filhos dos externos e irmão dos tags de mesmo patamar.

Exemplo: <pre><code>
&lt;div id="Ed"&gt;
&nbsp;&nbsp;&lt;div id="Edu"&gt; &lt;&minus;&minus;&excl; filho do Ed e irmão do Enio &minus;&minus;&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&lt;p id="Elô"&gt;&lt;&frasl;p&gt; &lt;&minus;&minus;&excl; filha do Edu e irmã do Helio &minus;&minus;&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&lt;p id="Helio"&gt;&lt;&frasl;p&gt; &lt;&minus;&minus;&excl; filho do Edu e irmão da Elô &minus;&minus;&gt;
&nbsp;&nbsp;&lt;&frasl;div&gt; 
&nbsp;&nbsp;&lt;spam id="Enio"&gt; &lt;&frasl;spam&gt; &lt;&minus;&minus;&excl; filho do Ed e irmão do Edu &minus;&minus;&gt; 
&lt;&frasl;div&gt;</code> </pre>

<a href="#inicio"> Voltar par o Início </a>



