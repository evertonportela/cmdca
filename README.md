# CMDCA - Considerações

# Negativas (Procurar resolver)

* Uma boa prática é utilizar o nome index.html para definir o arquivo principal do site, fiquei perdido entre os arquivos **novo.html, cmdca.html** e **site2.html**.
* Além disso, não é recomendado utilizar acentos ou simbolos especiais para renomear os arquivos de rota do site (**doaçoes.html, eleições.html**).
* Falhamos em responsividade, uma pessoa com Android ou iPhone tem uma visualização ruim do site.
* Conteúdos além de não obedecerem as diferentes configurações de tela, ficaram mal formatados, a exemplo em **doaçoes.html**, que o conteúdo de texto (corpo da página) não ficou centralizado.

O mesmo acontece em Documentos das Reuniões **documentos.html**

O mesmo acontece em Leis **leis.html**

Formatação de texto fugiu da estruturação padrão com algunas quebras de linha desnecessárias.

O mesmo acontece em Eleições **eleições.html**.

* Temos erros de ortografia/acentuação na **barra de menu principal**, no **Quem Somos**, no **Formulário de Contato**.
* Falhas de ligação em alguns hiperlinks, por exemplo, a partir do (Como Doar) **doaçoes.html** não é possível ir para (Notícias) **noticia.html** pela barra de menu principal. 

Assim como o contrário: (Notícias >> Como Doar).

A mesma coisa acontece em (Documentos Úteis >> Finanças)

A mesma coisa acontece em (Crianças e Adolescentes >> Finanças)

* Existe um submenu em Finanças -> **Funcionalidade** que não está linkado a nada.
* Existe um submenu em Documentos Úteis -> **Editais** que não está linkado a nada.
* Sobre padrão no uso de imagens, em **documentos.html** poderia ter utilizado a mesma imagem do topo do site.

* Barra de rolagem dentro do acordion ficou pouco agradável em **eleições.html**

* Em **login.html** o formulário de acesso restrito está passando dicas de preenchimentos distorcidas:

Da Página Inicial para a Página Eleições e na sequência ao clicar novamente em Eleições, o link leva para o arquivo **novo.html**. Que está inacabado e não dá opções de ir a nenhum outro lugar.

Onde se pede o nome, existe um exemplo de e-mail no placehold.

Onde se pede o email, existe um exemplo escrito senha e os caracteres estão ocultos.

* Barra de pesquisa não está funcional.

* Botões de acessibilidade não estão funcionais.

* Imagem LOGO do CMDCA não contém hiperlink para início do site.

* Faltou o rodapé do site (prometemos na reunião).

# Positivas (procurar aperfeiçoar)

* No geral conseguimos obter um padrão de cores, tamanho e tipo fonte. 

* Utilização acertiva de icones.

* o padrão de icones da página doações ficou bem aplicado, as cores foram bem aproveitadas, poderia ser utilizado tal padrão em todo o site.

* A ideia de aproveitar a imagem do CMDCA Rio foi legal, incrementando o simbolo de Santa Luzia do Itanhy. Mas é bom providenciar uma imagem original para evitar problemas de direitos autorais.

# Avaliação de Codificação
Considerações arquivo por arquivo

- **calendario.html** - Senti falta de mais detalhes e informações sobre os eventos do calendário. Também queria ver mais tag's de HTML5, utilizou muitas tag's de HTML4, usamos muitas DIVs. 
    - a tabela possui células de tamanho diferentes, deixando a página mal formatada e com aspecto feio.
    - (linha 9 - Falta de padrão no *title*) - Erro de português, esqueceu acentuação.
    - (linha 189 - descrição incoerente) - Está escrito no botão "voltar", porém ao clicar o link leva para a página inicial. Corrigir a descrição.
    - o css ficou visualmente bem organizado (mas precisa tomar cuidado com valores fixados com PX, uma opção é utilizar % ).
    - Pesquisar outros sites com calendário e pegar mais inspirações. Tem pouco conteúdo nessa página.

- **cmdca.html** - A começar o nome do arquivo deveria ser **index.html**. Para que o navegador entenda que se trata da página incial. Utilizou poucas tag's de HTML5. Alguns elementos funcionaram a responsividade, outros falharam e criaram barra de rolagem horizontal.
Problemas já citados:
    - (linha 5 - Falta de padrão no *title*)
    - (linha 27 - sem funcionalidade) - Os icones de acessibilidade não funcionam
    - (linha 47 - uso de (ç) simbolos especiais no href)
    - (linha 66 - uso de (çõ) simbolos especiais no href)
    - css - (linha 55 e linha 61 - usou o mesmo nome (pessoa) para o #ID e para a .CLASSE, isso pode confundir ).
    - o css ficou visualmente bem organizado (mas precisa tomar cuidado com valores fixados com PX, uma opção é utilizar % ).
    - Muito bom a intenção de fazer o menu adaptativo à tela com @media, mas precisa de revisão porque ainda falha.

- **conselheiros.html** - Não utilizou tag's de HTML5. Alguns elementos funcionaram a responsividade, outros falharam e criaram barra de rolagem horizontal. 
    - (linha 5 - falta de padrão no *title*)
    - (linha 77 - variável de pouco significado) - cx1 não é um bom nome de variável.
    - (linha 78 - variável de pouco significado) - cx2 não é um bom nome de variável.
    - (linha 79 - variável de pouco significado) - pres não é um bom nome de variável.
    - (linha 81 - variável de pouco significado) - img1 não é um bom nome de variável.
    - (linha 102 - erro de português) - na palavra *Instituto*
    - Os erros anteriores se repetem, consequência de *(Ctrl + C) e (Ctrl + V)* e pouca criatividade.
    - o CSS ficou visualmente bem organizado (mas precisa tomar cuidado com os nomes das classes e id's e com os valores fixados com PX, uma opção é utilizar % ). Interessante seguir o mesmo padrão ao renomear o arquivo CSS da mesma forma do arquivo HTML. 
    - Muito bom o uso de comentários no código do CSS.

- **contato.html** - Não utilizou tag's de HTML5. A responsividade funcionou em 30% das coisas. Fez o formulário sem utilizar a TAG FORM.
    - (linha 5 - falta de padrão no *title*)
    - Fez todo o formulário sem pelo meno um placeholder. 
    - O tipo de todos os campos são TEXT, não encontrei uma máscara de email ou de telefone.
    - O botão de enviar do formulário não tem pelo menos um SUBMIT.
    - o css ficou visualmente bem organizado (mas precisa tomar cuidado com valores fixados com PX, uma opção é utilizar % ). Interessante seguir o mesmo padrão ao renomear o arquivo CSS da mesma forma do arquivo HTML. 
    - Muito bom o uso de comentários no código do CSS. Mas achei erro de português. Sim, mesmo que no comentário, continua sendo erro. E o ideal seria colocar primeiro o comentário e depois escrever o código da classe.
    - *Preenchi o formulário, mas não recebi nenhum email de confirmação, não posso avaliar isso porque não sei se vocês aprenderam a configurar um form em situação de funcionamento real.*

- **criancas.html** -
    - (linha 5 - falta de padrão no *title*)

- **doacao.css** -
    este arquivo deveria estar na pasta *css*

- **doaçoes.html** - A começar pelo nome do arquivo, que não deveria ter acentuação
    - (linha 6 - falta de padrão no *title*)

- **documentos.html** -
    - Não existe *title* na página

- **eleições.html** - a começar pelo nome do arquivo, que não pode conter acentuação.
    - Não existe *title* na página.

- **foto.jgp** - o arquivo deveria estar na pasta imagens

- **galeria.html** -
    - (linha 7 - falta de padrão no *title*)

- **leis.html** -
    - (linha 6 - falta de padrão no *title*)

- **login.html** -
    - (linha 5 - falta de padrão no *title*)

- **galeria.html** -
    - (linha 7 - falta de padrão no *title*)

- **noticia.html** -
    - (linha 6 - falta de padrão no *title*)

- **novo.html** -
    - o arquivo deveria estar na pasta css

- **novo.html** -
    - (lina 2 - idioma) - Idioma da página se encontra em inglês. Quando o navegador abre, pergunta se eu desejo traduzir a página 🤷‍
    - Não existe *title* na página

