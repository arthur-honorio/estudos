##### Hypertext Markup Language

<h1 id="inicio">Links</h1>

Os hyperlinks são ligações entre documentos, eles referenciam endereços URL de outros documentos, fotos, mídias, sites, e é o torca o HTML um super arquivo capaz de se comunicar com servidores afim de fazer solicitações de recursos diversos pela web.

<h5><small>
Escolha abaixo o coneito que gostaria de ler:<br>
<a href="#ancora">Ancora</a> - <a href="#href">Href</a> - <a href="#absolutos">Caminhos Absolutos</a> - <a href="#relativos">Caminhos Relativos</a></small></h5>

<h2 id="ancora"> Ancora</h2>

A famosa tag <code>&lt;a&gt;&nbsp;&lt;&frasl;a&gt;</code>. Ela é utilizada para acessar, e gerar links clicáveis de direcionamento para conteúdos e páginas. Seu principal e imprescindível atributo é o <q>href</q>, sem ele a tag <code>&lt;a&gt;&nbsp;&lt;&frasl;a&gt;</code> simplesmente não tem utilidade, pois é no valor deste atributo que entra a URL ou o caminho de arquivo desejado.

Além do atributo acima citado, outros atributos, assim como os atributos globais, podem vir a ser úteis na ulitização desta tag. O atributo <q>download</q> por exemplo, transforma o link refernciado na tag num arquivo para download em vez de um site de acesso. Já o <q>target</q> serve para estipular se o link clicado abrirá o endereço na mesma página (se seu valor for nulo ou _self) ou se abrirá numa nova aba(se seu valor for _blank).

<a href="#inicio">Voltar ao Início</a>

<h2 id="href">Href</h2>

O href pode receber uma URL na web no formato "protocolo://domínio/path...", ou também receber o endereço local de navegação de diretórios de um arquivo em um sistema operacional.


<h3 id="absolutos">Caminhos absolutos</h3>

São as URL's que informam o caminho completo, desde a origem até o último dado que revela o recurso exato desejado, não considera o endereço do arquivo que está sendo editado. Qualquer um pode acessar um recurso com seu caminho absoluto, independentemente de onde esteja, a não ser que ele esteja em local reservado e/ou demande autorização.

<a href="#inicio">Voltar ao Início</a>


<h3 id="relativos">Caminhos relativos</h3>

É o caminho que usa como base onde está o arquivo a ser alterado. 
A sintaxe de navegação padrão apra acesso de recursos é:

- "./arquivo" ou "arquivo"
Quando o arquivo desejado está na mesma pasta que o arquivo que solicita acesso a ele.
- "./pasta_desejada/arquivo" ou "pasta_desejada/arquivo"
Quando o arquivo desejado estiver numa pasta na mesma pasta do arquivo que solicita acesso.
- "../"
É utilizado para subir uma pasta na hierarquia, acessar a pasta pai da pasta onde está o arquivo que solicita acesso a outro recurso. Ele pode ser inserido diversas vezes caso seja necessário voltar diversas vezes na hierarquia de diretórios do sistema.
    - - "../recurso_desejado"
    Acessa um recurso que está na pasta superior da hierarquia do sistema.
    - - "../pasta/recurso_desejado"
    Acessa um recurso que está numa pasta irmã da pasta atual, uma pasta presente na pasta superior na hierarquia da pasta atual.
    - - "../../recurso_desejado"
    Acessa um recurso que está duas pastas acima da pasta atual na hierarquia de diretórios.
    - - "../../pasta/recurso_desejado"
    Acessa um recurso que está numa pasta endereçada duas pastas acima da pasta atual na hierarquia de diretórios.

<a href="#inicio">Voltar ao Início</a>