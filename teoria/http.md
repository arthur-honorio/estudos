<h1 id="inicio">Hiper Text Transfer Protocol</h1>

Se divide em solicitação (requests) e respostas (responses), e lida com a troca de demandas/resultados entre um cliente e um servidor.

- Cliente: aquele que solicita um recurso a um servidor.

- Servidor: aquele que guarda recursos e os envia quando solicitado corretamente, dentro dos parametros exigidos. Em algumas situações um servidor pode ser um cliente.

<a href="#reqres">Requests/ Responses</a> -  <a href="#requests">Requests </a> - <a href="#methods">Methods</a> - <a href="#safe-idempotent">Safe/Idempotent</a>
<a href="#responses">Responses</a>

<h2 id="reqres"> Requests / Responses </h2>

Toda comunição no protocolo HTTP é feita através de pedidos e respostas.
O cliente faz um pedido e o servidor responde com o solicitado, se o pedido for válido, ou com a mensagem de erro, caso o pedido não seja válido.

Nas mensagens dessa comunicação existe uma divisão: Cabeçalho (headers) e Corpo (body).

- *HEADER:* No header, a linha inicial, conhecida como start-line, é a que indica o que deve ser feito no caso da request, ou o código do resultado da request no caso da response. Existem ainda muitos dados que são enviados e recebidos em formato *propriedade / valor* e que complementam a linha inicial. São dados como tamanho, formato de recurso, idade, localização de redirecionamento, entre outros.

- *BODY:* O corpo nem sempre está presente na mensagem - depende do verbo HTTP utilizado -, é separado do cabeçalho por uma linha em branco e seus conteúdos são fornecidos pelo cliente, na solicitação, ou pelo servidor, como mensagens de retorno, conteúdo a ser adicionado no servidor, entre outros.

<a href="#inicio">Voltar ao Início</a>

<h3 id="requests">Requests</h3>

A request é iniciada com o verbo (method) HTTP, seguido da URL e do protocolo, com a respectiva versão, que será utilizado na comunicação. 
Abaixo, sem linha em branco vêm os metadados, como o navegador que está fazendo a request e o tipo de arquivo que aguardado como response.

<a href="#inicio">Voltar ao Início</a>

<h4 id="methods">Methods</h4>

Seguem os principais verbos:
- *OPTION:* retorna quais os métodos estão disponíveis para interação com um recurso. 
- *GET:* solicita um recurso ao servidor, como o HTML duma página, por exemplo.
- *HEAD:* solicita somente o cabeçalho do recurso especificado.
- *POST:* cria e cadastra dados em um servidor.
- *PUT:* também cria e cadastra dados, mas é mais utilizado para fazer a substituição do conteúdo.
- *PATCH:* é mais utilizado para alterar somente uma parte de um recurso.
- *DELETE:* deleta o recurso especificado.
<br>

São classificados como seguros ou não seguros (safe) e idempotentes (idempotent) ou não idempotentes.

<ul id="safe-idempotent">
    <li><em>Safe:</em>são os métodos que solicitam somente uma leitura, não alteram nada no servidor. Os principais são: GET, HEAD e OPTION. Já os não seguros são aqueles que alteram informações no servidor, colocando, alterando ou  deletando dados do mesmo, por exemplo. Os principais são: POST, PUT, PATCH E DELETE.</li>
    <li><em>Idempotent:</em> são os métodos que recebem sempre a mesma resposta do servidor, independentemente da quantidade de solicitações feitas. O GET, o HEAD, o PUT e o DELETE sempre que utilizados receberão a mesma resposta do servidor. Os não idempotentes são aqueles que recebem respostas variáveis.</li>
</ul>
<a href="#inicio">Voltar ao Início</a>


<h3 id="responses">Responses</h3>

Começa com o protocolo solicitado na request seguido do status que indica o que foi retornado dessa solicitação.

São 5 categorias principais de status messages e cada categoria tem várias possibilidades diferentes:

- *100:* indica continuidade, a solicitação do cliente pode continuar seguindo sua rota.
- *200:* indica que deu tudo certo, o recurso foi encontrado e está sendo retornado.
- *300:* indica que foi necessário um redirecionamento para dar sequência à solicitação.
- *400:* indica erro na solicitação, seja no caminho, na autorização ou no recurso. O status mais conhecido é o "404 - not found".
- *500:* indica que o recurso existe, mas por um erro no servidor a ação não retornou o que foi solicitado.

<a href="#inicio">Voltar ao Início</a>