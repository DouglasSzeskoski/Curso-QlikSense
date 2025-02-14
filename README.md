# Curso-QlikSense
Curso de Qlik Sense, ferramenta para criação de BI

## Importar Dados
- Carregamos as tabelas em arquivos .cvs e Excel;
- Criamos e configuramos as relações entre as tabelas;
- Configuramos e alteramos os campos das tabelas do metadados.

## Criando Dimensões e Medidas
### DIMENSÕES
- Vamos criar as dimensões dentro do QLINK.
- Clicando no logo da QLIK voltamos à página inicial.
- Clicando nos três pontos da janela da aplicação escolha a opção Duplicar.
- Agora clique nos três pontos da cópia escolha Editar e entre com o nome BI da Empresa Suco de Frutas - Modelo de dados.
- Abra a aplicação original que estava sendo trabalhada BI da Empresa Suco de Frutas.
- Clique em Minha nova pasta e no botão Editar pasta.
- Agora clique em Itens mestres.
- Escolha a opção Dimensões e no botão Criar nova.
- Na janela Crias novas dimensões escolha Único.
- Em Filtras por tabela deixe a opção Todas as tabelas.
- Escolha o campo Fábrica, digite a descrição Dimensão Fábrica
- Escolha uma cor pela ordem das cores na tabela.
- O campo Fábrica foi criado e está na lista à esquerda.
- Clique em Criar nova.
- Escolha como dimensão Hierarquia.
- Adicione os campos na ordem do maior pro menor.
- No campo segmento chame de Segmento, descrição Dimensão segmento e escolha a próxima cor. E clique no botão Criar.
- Na mesma caixa de diálogo mantenha o botão em Hierarquia.
- Escolha os campos Região, Estado, Cidade e Cliente.
- Nomeie como Geográfica e descrição Dimensão geográfica com a próxima cor.
- Clique em Criar.
- Clique em Criar nova.
- Escolha como dimensão Hierarquia.
- Escolha os campos Tamanho e Produto.
- Nomeie como Tamanho e descrição Dimensão Tamanho com a próxima cor.
- Clique em Criar.
- Escolha como dimensão Hierarquia.
- Escolha os campos Sabor e Produto.
- Nomeie como Sabor e descrição Dimensão Sabor com a próxima cor.
- Clique em Criar.
- Escolha como dimensão Hierarquia.
- Escolha os campos Categoria, Marca e Produto.
- Nomeie como Produto e descrição Dimensão Produto com a próxima cor.
- Clique em Criar e Fechar.
- Clique em Criar nova.
- Escolha como dimensão Hierarquia.
- Escolha os campos Diretor, Gerente e Vendedor.
- Nomeie como Vendedor e descrição Dimensão Vendedor com a próxima cor.
- Clique em Criar e Fechar.
- Foram criadas as sete dimensões do metadados da Fábrica de sucos.

### MEDIDAS

- Abra o aplicativo.
- Na página principal clique em Minha Pasta.
- Clique agora em Editar pasta.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Faturamento em R$.
- Escolha a primeira cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão Sum[Faturamento em R$] e clique em Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Custo de Frete em R$.
- Escolha a proxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão Sum[Custo de Frete em R$] e clique em Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Imposto em R$.
- Escolha a proxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão Sum[Imposto em R$] e clique em Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Custo Fixo em R$.
- Escolha a próxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão Sum[Custo Fixo em R$] e clique em Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Custo Variável em R$.
- Escolha a próxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão Sum[Custo Variável em R$] e clique em Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Unidades Vendidas.
- Escolha a próxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão Sum[Unidades Vendidas] e clique em Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Quantidade Vendida em Litros.
- Escolha a próxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão Sum[Quantidade Vendidas em Litros] e clique em Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Meta de Faturamento em R$.
- Escolha a próxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão Sum[Meta de Faturamento em R$] e clique em Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Meta de Custo em R$.
- Escolha a próxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão Sum[Meta de Custo em R$] e clique em Aplicar e Criar.
- Vamos criar as medidas calculadas.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Faturamento Líquido em R$.
- Escolha a próxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão sum([Faturamento em R$]) - sum([Custo de Frete em R$]) - sum([Imposto em R$]) e clique em Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Margem em R$.
- Escolha a próxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão [Faturamento Líquido em R$] - sum([Custo Fixo em R$]) - sum([Custo Variável em R$]) e clique em Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Preço Médio R$ por Litro.
- Escolha a próxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão sum([Faturamento em R$]) / sum([Quantidade vendida em Litros])) e clique em Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Variação da Meta de Faturamento em %.
- Escolha a próxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão (([Faturamento Líquido em R$]/sum([Meta Faturamento em R$]) -1) * 100) e clique em Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Variação da Meta do Custo em %.
- Escolha a próxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão (((sum([Custo Fixo em R$]) + sum([Custo Variável em R$]))/sum([Meta de Custo em R$])) -1 ) * 100 e clique em - - - Aplicar e Criar.
- Na aba Medida clique em Criar nova.
- Na janela Criar nova medida entre com o nome e descrição Variação da Meta da Margem em %.
- Escolha a próxima cor.
- Em Expressão clique no fx e abra a área de edição da fórmula.
- Entre com a expressão (([Margem em R$]/ (sum([Meta Faturamento em R$]) - sum ([Meta de Custo em R$]))) -1 ) * 100 e clique em Aplicar     e Criar.
- Vamos montar agora a dimensão tempo.
- Clique novamente em Dimensões e Criar nova.
- Na janela Criar nova dimensões escolha Hierarquia e nomeie como Tempo.
- Escolha em Data na seguinte ordem Year, YearQuarter, YearMonth, Date.
- Selecione a cor roxa claro e clique em Criar e Fechar.
- Agora clique nos três pontos e escolha Visão geral do aplicativo.
- Com o botão direito do mouse na Minha nova pasta escolha a opção Duplicar.
- Clique nesta nova pasta e no botão Editar pasta.
- Verifique que os Itens mestres foram mantidos.
- Volte na Visão geral do aplicativo e exclua esta pasta criada.
- Clique no QLIK e clicando nos dois pontos da aplicação BI da Empresa Suco de Frutas escolha Duplicar.
- Renomeie a cópia da aplicação para BI da Empresa de Suco de Frutas - Criação das Medidas.

## CRIANDO AS VISÕES
- Vamos montar a primeira visão.
- Clique em Minha nova pasta.
- Na janela de Propriedades da pasta coloque Primeira visão com o QLIK em Título.
- Clique em Edição concluída e verifique que na página inicial aparece o título que foi modificado.
- Clique em Editar pasta.
- Quando clicar em Gráficos aparecem uma série de gráficos que podem ser usado.

  ### GRÁFICO DE KPI  
- Arraste KPI para a região superior esquerda.
- Clique em Itens mestres e Medidas e arraste a medida Faturamento em R$.
- Altere as dimensões do KPi.
- Clicando em Gráficos e escolhendo e arrastando o elemento Painel de filtro.
- Clique em Itens mestres e Dimensões e arraste Fábrica.
- Clicando em Edição concluída vai para a visão e ver as características do filtro de fábricas.
- Clique em Gráficos e arraste Gráfico de barra para a área da visão e ajuste o tamanho do gráfico na tela.
- Agora clique em Itens mestres e Dimensão e arraste a dimensão Tamanho para cima do gráfico.
- Em Medida escolha e arraste Faturamento para o gráfico de barra.
- Clique em Edição concluída e acompanhe as características da visão.
- Preste atenção na formatação quando for salvar a visão.

### GRÁFICO DE BARRAS
- Abra a pasta original e clique em Editar pasta.
- Selecione cada quadro e apague apertando a tecla Delete.
- Clicando em Gráficos e arraste Painel de filtro para a visão.
- Marcando Campos e abrir Data arraste Year para cima do filtro.'
- Ajuste o tamanho do quadro e clique em DataYear.
- Mude o Título para Selecione o ano.
- Clique em Edição concluída para ver como o filtro está funcionando.
- Clicando em Gráfico escolha e arraste Gráfico de barra para a visão.
- Em Campos arraste a dimensão Cidade para cima da caixa do gráfico.
- Selecionando Itens mestres e Medida e arraste Faturamento para cima do gráfico.
- Clique em Edição concluída para ver como o filtro funciona.
- Volte a editar a visão clicando em Editar a pasta.
- Com o gráfico selecionado aparecem algumas abas no lado direito da tela.
- Na aba classificação pode escolher a forma que será mostrado no gráfico.
- Trocando a ordem de classificação altera a forma do gráfico.
- Mantenha a ordem por Faturamento.
- Na aba Aparência mude o Título para Faturamento por Cidade e o Subtítulo para Dados expressos em reais.
- Podemos mudar a orientação do gráfico.
- Na aba Cores e legendas pode personalizar a cor.
- Altere o gráfico de acordo com o vídeo e escolha a melhor aparência para o gráfico.
- Clicando em Edição concluída e veja o funcionamento do filtro alterando o gráfico.
- Clique nos três pontos e escolha Visão geral do aplicativo.

### GRÁFICO DE LINHAS
- Clique em Editar pasta e clique no gráfico e aperte Delete para apagar o gráfico.
- Em Gráficos escolha Gráfico de linha.
- Em Campos e Data escolha YearMonth e arraste para o gráfico.
- Escolha como dimensão.
- Em Medidas escolha e arraste Faturamento para o gráfico.
- Com o gráfico selecionado vá na aba lateral direita e escolha em Complementos e Manipulação de dados desmarque a opção Incluir valores - zero.
- Em Aparência/Geral coloque o título Faturamento ao longo do tempo e o subtítulo Valores expressos em reais.
- Troque a cor do gráfico.
- Em Estilo mude as características da linha.
- lique em Edição concluída.
- Veja como ficou o gráfico.

### GRÁFICO DE PIZZA
- Clique em Editar pasta e clique no gráfico e aperte Delete para apagar o gráfico.
- Em Gráficos escolha Gráfico de pizza. Ajuste o gráfico.
- Em Campos escolha Categoria e arraste para o gráfico.
- Em Medidas escolha e arraste Faturamento para o gráfico.
- Com o gráfico selecionado em Aparência/Geral coloque o título Distribuição de faturamento por categoria e o subtítulo Valores expressos em reais.
- Clique em Edição concluída.
- Veja que pode girar o gráfico e o filtro continua a funcionar.

### MAPAS
- Mais uma vez clique em Editar pasta, selecione o gráfico e aperte Delete para apagar o gráfico.
- Em Gráficos escolha Mapa e agora ajuste o gráfico.
- Em Campos escolha Estado e arraste para o gráfico.
- Escolha a opção Adicionar como camada de área. Não mostra todos os estados.
- Arraste Sigla para cima do gráfico e escolha Adicionar "Sigla" como localização". Também não mostra todos os estados.
- Clique nos três pontos ao lado do logo e escolha Gerenciador de dados.
- Abra a tabela Dim_Cliente clique em Editar tabela.
- Clique em Adicionar campo e Campo calculado.
- Dê o nome de Sigla_Estado.
- Entre com a expressão if(Sigla = 'GO', Sigla, if(Sigla = 'DF', Sigla, Estado) e clique Criar e Carregar dados.
- Clique nos três pontos e selecione Visão geral do aplicativo.
- Selecione o gráfico e aperte Delete para apagar o mapa.
- Em Gráficos escolha Mapa e ajuste o gráfico.
- Em Campos escolha Sigla_Estado e arraste para o gráfico.
- Na aba lateral direita escolha Cores e selecione Por medida.
- Escolha como medida o campo Faturamento.
- Clique em fx e use a medida Faturamento em R$.
- Altere a Cor do contorno para preto e melhore as linhas.
- Dê um clique no título e altere para Faturamento distribuído por estados.
- Clique em Edição concluída.
- Veja o que altera no gráfico e que o filtro continua a funcionar.

### MAPA DE BOLHAS
- Em Campos escolha Cidade e arraste para o gráfico. Escolhe uma nova camada de dados Adicionar como camada de ponto.
- Na aba da direita clique em Camadas e Cidade** e abra Tamanho e forma e aumente o tamanho do círculo.
- Em Dimensionar por escolha o campo Margem em R$.
- Em Cores troque a cor da bolha e do contorno.
- Clique em Edição concluída.
- Veja que pode girar o gráfico e o filtro continua a funcionar.
- Clique no logo QLIK e duplique a aplicativo e nomeie como BI da Empresa de Suco de Fruta - Mapa Bolha.

### MAPA DE ÁRVORE
- Em Gráficos escolha Mapa de árvore e ajuste o gráfico.
- Em Campos escolha Região como dimensão e arraste para o gráfico.
- Escolha como medida o campo Faturamento em Itens mestres.
- Clique em Incluir e escolha Categoria.
- Com duas dimensões o gráfico mostra que a área maior representa a região e os retângulos menores a categoria.
- Em Aparência altere o Título para Distribuição de Faturamento por Região e Categoria.
- Clique em Edição concluída.

### MOSTRADORES / APONTADORES
- Em Gráficos escolha Mostrador. Ajuste o gráfico.
- Em Itens mestres/Medidas escolha e arraste Variação da Meta do Faturamento em % para cima do gráfico.
- Com o gráfico selecionado em Aparência/Geral coloque o título Variação da Meta do Faturamento.
- Em Apresentação coloque nos limtes de -50 a +50.
- Clique na opção Usar segmento e desmarque Usar biblioteca.
- Agora clique em Adicionar limite e coloque como -10.
- Clique em cima da primeira área para trocar a cor para vermelho.
- Agora clique em Adicionar limite e coloque como 10.
- Clique em cima da segunda área para trocar a cor para amarelo.
- Finalmente clique em Adicionar limite e coloque como 50.
- Clique em cima da terceira área para trocar a cor para verde. Pode ser usado o gradiente para escolher a cor.
- Clique em Edição concluída.
- Veja que pode alterar o gráfico e o filtro continua a funcionar.

### DISPERSÃO
- Clicando em Itens mestres/Medidas escolha Criar nova.
- Coloque no nome Margem Unitária (R$/Litros) e acrescente a expressão usando as medidas Margem em R$/Quantidade Vendida em Litros. - 
- Escolha uma cor e clique Criar.
- Em Gráficos escolha Dispersão. Ajuste o tamanho do gráfico.
- Em Campos escolha Produto e arraste para o gráfico.
- Em Itens mestres/Medidas escolha e arraste Faturamento em R$ para o Eixo X no gráfico.
- Em Itens mestres/Medidas escolha e arraste Margem Unitária (R$/Litros) para o Eixo Y no gráfico.
- Clique no título do gráfico e altere para Comparação entre Faturamento e Margem Unitária.
- Clique em Edição concluída.

### TABELA
- Em Gráficos escolha Tabela. Ajuste o gráfico.
- Em Campos escolha Estado, Cliente e arraste para o gráfico.
- Em Itens mestres/Medidas escolha e arraste Faturamento em R$ para o gráfico.
- Na aba direita escolha Faturamento em R$ desmarque a formatação automática.
- Em Formato numérico escolha Moeda. Troque o padrão de formato.
- Com o gráfico selecionado em Aparência/Geral coloque o título Faturamento por Estado e Cliente .
- Em Apresentação desmarque Totais. Escolha em Posição a opção Inferior
- Clique em Edição concluída.

### USANDO AS DIMENSÕES / DRILLDOWN  
- Em Gráficos escolha Gráfico de pizza.
- Em Itens mestres/Dimensões escolha Geográfica e arraste para o gráfico.
- Em Medidas escolha e arraste Faturamento em R$ para o gráfico.
- Ajuste o gráfico.
- Em Gráficos escolha Gráfico de barra.
- Em Itens mestres/Dimensões escolha Produto e arraste para o gráfico.
- Em Medidas escolha e arraste Faturamento em R$ para o gráfico.
- Com o segundo gráfico selecionado clique em Aparência e escolha a opção Estilo Horizontal e na Classificação coloque Faturamento em R$ no topo da lista.
- Nomeie o gráfico de pizza como Faturamento por Geografia e no de barra Faturamento por Produto.
- Clicando nas partes dos gráficos automaticamente são criados filtros.

### DASHBOARDS
- Vamos escolher as pastas que farão parte do Dashboard.
- Clique no mapa Gráfico de Barras.
- Selecionando o gráfico clique nos três pontos e escolha a opção Adicionar aos itens mestres.
- Mantenha o nome Faturamento por Cliente e clique em Incluir.
- Clicando nos três pontos ao lado do logo QLIK escolha a opção Visão geral do aplicativo.
- Escolha o Gráfico de Pizza.
- Com o gráfico selecionado clique nos três pontos e escolha a opção Adicionar aos itens mestres. E Incluir.
- Novamente clique nos três pontos ao lado do logo QLIK escolha a opção Visão geral do aplicativo.
- Agora clique para abrir a pasta Mostradores.
- Com o gráfico selecionado clique nos três pontos e escolha a opção Adicionar aos itens mestres. E Incluir.
- Agora clique nos três pontos ao lado do logo QLIK escolha a opção Visão geral do aplicativo.
- Crie e abra uma nova pasta com o nome Dashboard.
- Clique em Editar pasta.
- Em Gráficos escolha o campo Painel de Filtro.
- Em Campos arraste Data/Year e Fábrica para cima do filtro.
- Ajuste o filtro com uma linha.
- Na aba da direita em Data/Year troque o título para Ano.
- Abra a aba Visualizações e arraste todas para a área da visão.
- Aumento o gráfico de barras para ocupar a área da esquerda e coloque na direita a pizza sobre o mostrador.
- Clique em Edição concluída para ver a exibição.
- Clicando em Ano ou Fábrica os gráficos são sensibilizados.
- Pode fechar os filtros criados automaticamente para salvar a posição original.

### CRIANDO UMA NARRATIVA
- Abra o aplicativo mestre BI de Empresa de Sucos de Frutas e a pasta Dashboard.
- Clicando no filtro Ano escolha 2012.
- Nos três pontos do Mostrador escolha Snapshots de narrativa e depois Tirar snapshot.
- Na janela aberta escreva 1 - Meta de Faturamento 2012 e clique em Salvar.
- Clicando no filtro Ano escolha 2015.
- Nos três pontos do Mostrador escolha Snapshots de narrativa e depois Tirar snapshot.
- Na janela aberta escreva 2 - Meta de Faturamento 2015 e clique em Salvar.
- Clicando nas cidades do gráfico de barras pode ver qual cidade ajudou na recuperação da meta.
- Escolha a cidade Campinas.
- Nos três pontos do Mostrador escolha Snapshots de narrativa e depois Tirar snapshot.
- Na janela aberta escreva 3 - Meta de Faturamento em 2015 para Campinas e clique em Salvar.
- Clicando nas cidades do gráfico de pizza pode ver qual produto ajudou na recuperação da meta.
- Escolha o produto Mate no gráfico de pizza.
- Nos três pontos do Mostrador escolha Snapshots de narrativa e depois Tirar snapshot.
- Na janela aberta escreva 4 - Meta de Faturamento em 2015 para Campinas e Mate e clique em Salvar.
- Clicando no botão Pastas escolha Gráfico de Linhas. O gráfico de linha é aberto. Acompanhe a explicação do vídeo.
- Nos três pontos do gráfico e escolha Snapshots de narrativa e depois Tirar snapshot.
- Na janela aberta escreva 5 - Sazonalidade das vendas de mate em 2015 em Campinas e clique em Salvar.
- Clique no botão Narrativa.
- Na janela aberta clique nq A** e arraste **Titulo para área em branco. Escreva Análise da Meta de Faturamento.
- Clique no botão Biblioteca de Snapshot e escolha o primeiro.
- Clicando no lápis pode alterar algum formato do snapshot. Retire o título, coloque Somente rótulos e em Escalas escolha estreito.
- Clicando no A** escolha **Paragrafo entre com o texto do parágrafo. Formate o parágrafo.
- Acrescente um novo snapshot clicando no botão Biblioteca de snapshot. Arraste o segundo para dentro da área em branco.
- Clicando no lápis pode alterar algum formato do snapshot. Retire o título, coloque Somente rótulos e em Escalas escolha estreito.
- Clicando no A** escolha **Paragrafo entre com o texto do parágrafo. Formate o parágrafo.
- Clicando com o botão direito do mouse no slide escolha a opção Duplicar.
- Apague todos os componentes selecionando e apertando a tecla Delete.
- Clique no botão Biblioteca de Snapshot e escolha o número 3.
- Copie as características do snapshoot.
- Copie e cole o texto dos outros mostradores. Altere o texto
- Acrescente um novo snapshot clicando no botão Biblioteca de snapshot. Arraste o quarto para dentro da área em branco.
- Edite e deixe com as mesmas características dos outros mostradores.
- Copie cole o texto anterior. Edite o parágrafo.
- Clicando com o botão direito do mouse no slide escolha a opção Duplicar.
- Apague todos os componentes selecionando e apertando a tecla Delete.
- Clicando no lápis altere o do snapshot. Retire o título, coloque Somente rótulos e em Escalas escolha estreito.
- Copie cole o texto anterior. Edite o parágrafo.
- Clique em Histórias para verificar se foi criada.
- Clique em Reproduzir a história.

## SCRIPT

### BUSCAR ULTIMAS 12 PLANILHAS
  Criar uma script para automatizar o upload de planilhas, para que seja feito upload somente dos ultimos 12 meses a partir da data de planilha mais recente.

LET v_Diretorio_CSV = 'lib://Formação Qlik:DataFiles';

FOR Each v_CSVArquivos in FileList('$(v_Diretorio_CSV)/*.CSV')
  //Trace $(v_CSVArquivos);
  Temp_Lista_Arquivos:
    LOAD
    	'$(v_CSVArquivos)' AS Arquivo_nome_full,
        SubField('$(v_CSVArquivos)', '/',4) AS Arquivo,
        SubField(SubField('$(v_CSVArquivos)', '/',4),'_',2) 
        	& REPLACE(SubField(SubField('$(v_CSVArquivos)', '/',4),'_',3),'.CSV','') AS Ano_Mes_Arquivo_2,
        If(Num#(REPLACE(SubField(SubField('$(v_CSVArquivos)', '/',4),'_',3),'.CSV','')) <= 9,
        	'0' & (REPLACE(SubField(SubField('$(v_CSVArquivos)', '/',4),'_',3),'.CSV','')),
        (REPLACE(SubField(SubField('$(v_CSVArquivos)', '/',4),'_',3),'.CSV',''))) AS Mes_Arquivo,
        Date(Date#(SubField(SubField('$(v_CSVArquivos)', '/',4),'_',2) & If(Num#(REPLACE(SubField(SubField('$(v_CSVArquivos)', '/',4),'_',3),'.CSV','')) <= 9,
        	'0' & (REPLACE(SubField(SubField('$(v_CSVArquivos)', '/',4),'_',3),'.CSV','')),
        (REPLACE(SubField(SubField('$(v_CSVArquivos)', '/',4),'_',3),'.CSV',''))),'YYYYMM')) AS Ano_Mes_Arquivo
        AutoGenerate 1;
        
Next v_CSVArquivos;

temp:
LOAD 
	date(MAX(Ano_Mes_Arquivo)) AS Max_Data,
    AddMonths(date(MAX(Ano_Mes_Arquivo)), - 11) AS Min_Data
Resident Temp_Lista_Arquivos;

Let Maior_mes = Peek('Max_Data');
Let Menor_mes = Peek('Min_Data');

NoConcatenate
Final_Lista_Arquivos:
LOAD * Resident Temp_Lista_Arquivos 
Where Ano_Mes_Arquivo >= '$(Menor_mes)' 
	AND Ano_Mes_Arquivo <= '$(Maior_mes)';

DROP TABLE Temp_Lista_Arquivos;

For vArquivo = 1 to NoOfRows('Final_Lista_Arquivos')
	Let vArquivoNomeCarga = Peek('Arquivo_nome_full', vArquivo -1, 'Final_Lista_Arquivos');
	trace '$(vArquivoNomeCarga)';

Next vArquivo

LOAD
    cpf,
    data_venda,
    matricula,
    codigo_do_produto,
    quantidade,
    faturamento
FROM [$(vArquivoNomeCarga)]
(txt, utf8, embedded labels, delimiter is ';', msq);

DROP TABLE Final_Lista_Arquivos;
