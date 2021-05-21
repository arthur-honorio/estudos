# Hiper Text Transfer Protocol.

Se divide em requisições e respostas, e lida com a troca de demandas/resultados entre um cliente e um servidor.

- Cliente: aquele que solicita um recurso a um servidor.

- Servidor: aquele que guarda recursos e os envia quando solicitado corretamente, dentro dos parametros exigidos. Em algumas situações um servidor pode ser um cliente.

## Requests / Responses

Toda comunição no protocolo HTTP é feita através de pedidos e repsostas. O cliente faz um pedido e o servidor responde com o solicitado, se o pedido for válido, ou com a mensagem de erro, caso o pedido não seja válido.

Nas mensagens dessa comunicação existe uma divisão: Cabeçalho (headers) e Corpo (body).

No header, a linha inicial, conhecida como start-line, é a que indica o que deve ser feito no caso da request, ou o código do resultado da request no caso da response. Existem ainda muitos dados que são enviados e recebidos em formato *propriedade / valor* e que complementam a linha inicial. São dados como tamanho, formato de recurso, idade, localização de redirecionamento, entre outros.

O corpo nem sempre está presente na mensagem - depende do verbo HTTP utilizado -, é separado do cabeçalho por uma linha em branco e contém conteúdos fornecidos pelo cliente ou pelo servidor, como mensagens de retorno, conteúdo a ser adicionado no servidor, entre outros.

### Request

A request é iniciada com o verbo (method) HTTP, seguido da URL e do protocolo, com a respectiva versão, que será utilizado na comunicação. 
Abaixo, sem linha em branco vêm os metadados, como o navegador que está fazendo a request e o tipo de arquivo que aguardado como response.

##### Methods

São classificados como seguros ou não seguros (safe) e idempotentes (idempotent) ou não idempotentes.

- *Safe:* são os métodos que solicitam somente uma leitura, não alteram nada no servidor. Os principais são: GET, HEAD e OPTION. Já os não seguros são aqueles que alteram informações no servidor, colocando, alterando ou  deletando dados do mesmo, por exemplo. Os principais são: POST, PUT, PATCH E DELETE.
- *Idempotent:* são os métodos que recebem sempre a mesma resposta do servidor, independentemente da quantidade de solicitações feitas. O GET, o HEAD, o PUT e o DELETE sempre que utilizados receberão a mesma resposta do servidor. Os não idempotentes são aqueles que recebem respostas variáveis.

Seguem os principais verbos:
- *OPTION:* retorna quais os métodos estão disponíveis para interação com um recurso. 
- *GET:* solicita um recurso ao servidor, como o HTML duma página, por exemplo.
- *HEAD:* solicita somente o cabeçalho do recurso especificado.
- *POST:* cria e cadastra dados em um servidor.
- *PUT:* também cria e cadastra dados, mas é mais utilizado para fazer a substituição do conteúdo.
- *PATCH:* é mais utilizado para alterar somente uma parte de um recurso.
- *DELETE:* deleta o recurso especificado.

### Response

Começa com o protocolo solicitado na request seguido do status que indica o que foi retornado dessa solicitação.

São 4 categorias principais de status messages e cada categoria tem várias possibilidades diferentes:

- *100:* indica continuidade, a requisição do cliente pode continuar seguindo sua rota.
- *200:* indica que tudo deu certo, o recurso foi encontrado e está sendo retornado.
- *300:* indica que foi necessário um redirecionamento para dar sequência à solicitação.
- *400:* indica erro na requisição, seja no caminho, na autorização ou no recurso. O status mais conhecido é o "404 - not found".
- *500:* indica que o recurso existe, mas por um erro no servidor a ação não retornou o que foi solicitado.