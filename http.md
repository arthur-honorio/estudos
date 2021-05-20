# Anotações sobre http

## Hiper Text Transfer Protocol.

Se divide em requisições e respostas, e lida com a troca de demandas/resultados entre um cliente e um servidor.

- Cliente: aquele que solicita um recurso a um servidor.

- Servidor: aquele que guarda recursos e os envia quando solicitado corretamente,
dentro dos parametros exigidos. Em algumas situações um servidor pode ser um cliente.

<strong> URI </strong> Uniform Resource Indentity, tem dois tipos de identificador:

- <strong> URL </strong> Uniform Resource Locator: fornece o local onde o recurso está armazenado.
Este 'endereço' é separado em elementos menores para especificar exatamente a localização. Destes elemetos, 2 são obrigatórios: o Protocolo e o Domínio.
<strong> Protocolo </strong>: é o primeiro elemento do URL e indica qual o protocolo utilizado para acessar o recurso desse endereço. Ele adicionado automaticamente quando não especificado pelo usuário.
<strong> Domínio </strong>: é o nome ao qual o IP é assossiado. Ex.: rocketseat.com, google.com, youtube.com .
<strong> TLD </strong>: Top Level Domain é o fim do domínio. Ex. com, br, com.br, uk, space.

Outros elementos são opcionais:
- <strong> Subdomínio </strong>: alguns url's exitem o subdomínio, mas ele não é um elemento obrigatório a todos. Ex.: www.
- <strong> Path </strong>: é o que vem depois do TLD. Começa com uma barra "/" e especifíca o caminho exato para encontrar o recurso. Ex.: rocketseat.com.br/blog.

Obs.: A barra "/" indica a home do domínio digitado e é incluída automaticamente pelo navegador.

- <strong> URN </strong> Uniform Resource Name: é um parâmetro único para indicar o nome único do recurso, não informa a localização do mesmo.
Ex.: isbn (é um número único de registro internacional que é associado a qualquer publicação cadastrada neste banco de dados).

