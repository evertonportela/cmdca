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

Onde se pede o nome, existe um exemplo de e-mail no placehold.

Onde se pede o email, existe um exemplo escrito senha e os caracteres estão ocultos.

Da Página Inicial para a Página Eleições e na sequência ao clicar novamente em Eleições, o link leva para o arquivo **novo.html**. Que está inacabado e não dá opções de ir a nenhum outro lugar.

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
    - (linha 5 - Falta de padrão no *title*).
    - (linha 27 - sem funcionalidade) - Os icones de acessibilidade não funcionam.
    - (linha 32 - Erro de português) - Falta de acentuação em *Noticias*.
    - (linha 39 - Erro de português) - Falta de acentuação em *Calendario*.
    - (linha 47 - uso de (ç) simbolos especiais no href).
    - (linha 51 - Erro de português) - Falta de acentuação em *Uteis*.
    - (linha 59 - Erro concordância) - Falta de concordância com plural em *Adolescente*.
    - (linha 66 - uso de (çõ)) -  simbolos especiais no href.
    - (linha 73 - sem funcionamento) - Não será penalizado porque não sei se foram ensinados a configurar essa funcionalidade.
    - (linha 83 - variável ID poderia ter um nome melhor)
    - (linha 86 - variável ID poderia ter um nome melhor)
    - (linha 90 - variável ID poderia ter um nome melhor)
    - (linha 103 - variável CLASS poderia ter um nome melhor)
    - (linha 104 - variável ID poderia ter um nome melhor)
    - (linha 108 - variável CLASS poderia ter um nome melhor)
    - (linha 109 - variável ID poderia ter um nome melhor)
    - (linha 113 - variável CLASS poderia ter um nome melhor)
    - (linha 114 - variável ID poderia ter um nome melhor)
    - (linha 119 - variável CLASS poderia ter um nome melhor)
    - (linha 121 - variável CLASS poderia ter um nome melhor)
    - CSS - (linha 55 e linha 61 - usou o mesmo nome (pessoa) para o #ID e para a .CLASS, isso pode confundir ).
    - CSS - (linas 5-9) não utilizadas.
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
    - Muito bom o uso de comentários no código do CSS. Mas a palavra *ultilizada* foi escrita errada e ficou repetida várias no código vezes.

- **contato.html** - Não utilizou tag's de HTML5. A responsividade funcionou em 30% das coisas. Fez o formulário sem utilizar a TAG FORM.
    - (linha 5 - falta de padrão no *title*)
    - (linhas 77-83) - a aplicação de LABEL é indicada para legenda de um campo de formulário. Espera-se utilizar input após usar a LABEL. Foi usado de forma equivocada. 
    - Fez todo o formulário sem pelo meno um placeholder. 
    - O tipo de todos os campos são TEXT, não encontrei uma máscara de email ou de telefone.
    - O botão de enviar do formulário não tem pelo menos um SUBMIT.
    - o css ficou visualmente bem organizado (mas precisa tomar cuidado com valores fixados com PX, uma opção é utilizar % ). Interessante seguir o mesmo padrão ao renomear o arquivo CSS da mesma forma do arquivo HTML. 
    - Muito bom o uso de comentários no código do CSS. Mas achei erro de português. Sim, mesmo que no comentário, continua sendo erro. E o ideal seria colocar primeiro o comentário e depois escrever o código da classe.
    - *Preenchi o formulário, mas não recebi nenhum email de confirmação, não posso avaliar isso porque não sei se vocês aprenderam a configurar um form em situação de funcionamento real.*

- **criancas.html** - Comentou hein! Mas tá bom.
    - (linha 5 - falta de padrão no *title*).
    - (linha 79) - trecho de texto com erro de digitação *cuida especificamente dos direitos "dos" das crianças*.
    - (linha 87) - trecho com erro na quebra de linha.
    - (linha 88) - trecho com erro na quebra de linha.
    - (linha 89) - trechos com erro na quebra de linha.
    - CSS - o css ficou bom, tratando dos tamanhos de forma percentual, só não ficou top porque a imagem quebrou a responsividade quando eu mudei o tamanho da tela. Também ficou bem comentado, observar que na linha 7 faltou letra na palavra *alinhar*.

- **doacao.css** -
    Este arquivo deveria estar na pasta *css*. Ou deveria ter sido apagado já que não está sendo usado.

- **doaçoes.html** - A começar pelo nome do arquivo, que não deveria ter acentuação.
    - (linha 2 - idioma) - Idioma da página se encontra em inglês. Quando o navegador abre, pergunta se eu desejo traduzir a página 🤷‍.
    - (linha 6 - falta de padrão no *title*).
    - (linha 78 - variável de pouco significado) - a-b não é um bom nome de variável.
    - (linha 91 - erro de digitação) - no trecho *E-mail ou numero de celular*

- **documentos.html** -
    - Não existe *title* na página.
    - (linha 76) - não é aconselhado usar a palavra reservada "div", pode confundir e dar problema no CSS.
    - (linha 77 - variável de pouco significado) - img não é um bom nome de variável para ID.

- **eleições.html** - a começar pelo nome do arquivo, que não pode conter acentuação.
    - Não existe *title* na página.
    - (linha 2 - idioma) - idioma da página está em inglês.
    - (linha 9) - link para arquivo css que não está sendo utilizado na página.
    - (linha 79 - variável de pouco significado) - img não é um bom nome de variável para CLASS, pode causar problemas no lado do CSS.
    - (linha 95 - erro de digitação) - no trecho *em dia e documento com fot*

- **foto.jgp** - o arquivo deveria estar na pasta imagens.

- **galeria.html** - o arquivo nem está sendo usado no site.
    - (linha 7 - falta de padrão no *title*).

- **leis.html** - Seria legal usar mais tag's de HTML5.
    - (linha 6 - falta de padrão no *title*)
    - (linha 77 - variável de pouco significado) - 'cm' não é um bom nome de variável para CLASS, pode causar problemas no lado do CSS.
    - (linha 79 - variável de pouco significado) - 'c' não é um bom nome de variável para CLASS, pode causar problemas no lado do CSS.
    - (linha 80) - trecho com erro de digitação *DECRETO 1066-2018 COMPOSIÇÃO DO CMDI*
    - (linha 92) - trecho com erro de digitação, consequência do *Ctrl + C*, em *de Criação do CMDCA-Rio*

- **login.html** -
    - (linha 5 - falta de padrão no *title*)
    - (linha 20-21) - O label solicita o nome da pessoa, mas o placeholder exemplifica um e-mail. 
    - (linha 25-26) - O label solicita o e-mail da pessoa, mas o placeholder exemplifica a senha. E era bom deixar a senha com os caracteres ocultados.
    - (linha 37) - A descrição do botão deveria ser *Página Inicial*.

- **noticia.html** -
    - (linha 5 - falta de padrão no *title*).
    - (linha 78 - variável de pouco significado) - 'div1' não é um bom nome de variável para CLASS, pode causar problemas no lado do CSS.
    Porque utilizar uma classe para cada notícia, se no fim todas recebem praticamente os mesmos parâmetros. Classe tem o objetivo de ser feito uma vez e reaproveitado durante o código, não precisaria criar img1, img2 e img3...    

- **novo.css** -
    - o arquivo deveria estar na pasta css.

- **novo.html** -
    - (linha 2 - idioma) - Idioma da página se encontra em inglês. Quando o navegador abre, pergunta se eu desejo traduzir a página 🤷‍.
    - Não existe *title* na página.

- **projetos.html** -
    - (linha 5 - falta de padrão no *title*).

- **site2.html** -
    - (linha 5 - falta de padrão no *title*).
    - Não é uma boa prática usar a estilização CSS dentro da própria página.

- **somos.html** -
    - (linha 4 - falta de padrão no *title*) - existe, mas é como se não existisse.