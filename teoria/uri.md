# URI
Uniform Resource Indentity, tem dois tipos de identificador:

## URL
Uniform Resource Locator: fornece o local onde o recurso está armazenado.
Este 'endereço' é separado em elementos menores para especificar exatamente a localização. Destes elemetos, 2 são obrigatórios: o Protocolo e o Domínio.

- *Protocolo:* é o primeiro elemento do URL e indica qual o protocolo utilizado para acessar o recurso desse endereço. Ele adicionado automaticamente quando não especificado pelo usuário.
- *Domínio:* é o nome ao qual o IP é assossiado. Ex.: rocketseat.com, google.com, youtube.com .
- *TLD:* Top Level Domain é o fim do domínio. Ex. com, br, com.br, uk, space.

Outros elementos são opcionais:
- *Subdomínio:* alguns url's exitem o subdomínio, mas ele não é um elemento obrigatório a todos. Ex.: www.
- *Path:* é o que vem depois do TLD. Começa com uma barra "/" e especifíca o caminho exato para encontrar o recurso. Ex.: rocketseat.com.br/blog.
        Obs.: A barra "/" indica a home do domínio digitado e é incluída automaticamente pelo navegador.
- *Paramêtros:* são dados passados no URL para se chegar a um recurso específico. Ex.: youtube.com/watch?v=adaslej
- *Porta:* é uma localização onde cada protocolo específico pode executar seu script, sua comunicação. É um número que vem depois de : e aparece após do domínio, seja ele um ip ou um nome de domínio.
- *Âncora:* acessa uma parte específica de um recurso disponível do domínio informado anteriormente.


## URN 
Uniform Resource Name: é um parâmetro único para indicar o nome único do recurso, não informa a localização do mesmo.
Ex.: isbn (é um número único de registro internacional que é associado a qualquer publicação cadastrada neste banco de dados).
