# Campinas Election - 2020

=======================================

Project to analyse proposals from mayor candidates to 2020 elections in Campinas-SP, Brazil.
- Campinas: https://en.wikipedia.org/wiki/Campinas
- Campinas-Official: http://www.campinas.sp.gov.br/
- Data Source: http://divulgacandcontas.tse.jus.br/divulga/#/municipios/2020/2030402020/62910/candidatos
Project developed on Jupyter Notebook.

========================================

## Propostas
Projeto para analisar propostas de candidatos a prefeito de Campinas-SP em 2020.

Propostas incluídas no registro de candidatura enviada ao TSE por cada prefeito.

Excluindo 1 caso: Dr. Hélio que usou scan e fotos no pdf enviado


"Nome Completo"|"Nome Urna"|"Cargo"|"Número"|"Partido"|"Coligação"|"Situação"|"Situação Pós-Pleito"|"Proposta"
-------------- | --------- | ----- | ------ | ------- | --------- | -------- | ------------------- | ---------
"ALESSANDRA RIBEIRO MARTINS"|"ALESSANDRA RIBEIRO"|"Prefeito"|65|"PC do B"|"PC do B"|"Aguardando julgamento"|"Concorrendo"|"PDF"
"ANDRÉ LUIZ DE CAMARGO VON ZUBEN"|"ANDRÉ VON ZUBEN"|"Prefeito"|23|"CIDADANIA"|"CAMPINAS MERECE MAIS"|"Aguardando julgamento"|"Concorrendo"|"PDF"
"ARTUR CASSEB ORSI"|"ARTUR ORSI"|"Prefeito"|55|"PSD"|"PSD"|"Aguardando julgamento"|"Concorrendo"|"PDF"
"DARIO JORGE GIOLO SAADI"|"DARIO SAADI"|"Prefeito"|10|"REPUBLICANOS"|"PRONTOS PRA CAMPINAS"|"Aguardando julgamento"|"Concorrendo"|"PDF"
"TERESINHA DE CARVALHO"|"DELEGADA TERESINHA"|"Prefeito"|14|"PTB"|"MUDANÇA PRA VALER"|"Aguardando julgamento"|"Concorrendo"|"PDF"
"HÉLIO DE OLIVEIRA SANTOS"|"DR HÉLIO"|"Prefeito"|12|"PDT"|"PDT"|"Aguardando julgamento"|"Concorrendo"|"SCAN"
"LAURA LEAL DE CASTRO"|"LAURA LEAL"|"Prefeito"|16|"PSTU"|"PSTU"|"Aguardando julgamento"|"Concorrendo"|"PDF"
"PEDRO TOURINHO DE SIQUEIRA"|"PEDRO TOURINHO"|"Prefeito"|13|"PT"|"DEMOCRACIA, DIREITOS E LIBERDADE"|"Aguardando julgamento"|"Concorrendo"|"PDF"
"AHMED TARIQUE TOMBOUCTOU AGIO"|"PROF AHMED TARIQUE AGIO"|"Prefeito"|33|"PMN"|"PMN"|"Aguardando julgamento"|"Concorrendo"|"PDF"
"RAFAEL FERNANDO ZIMBALDI"|"RAFA ZIMBALDI"|"Prefeito"|22|"PL"|"MAIS POR CAMPINAS, MELHOR PRA VOCÊ"|"Aguardando julgamento"|"Concorrendo"|"PDF"
"ROGERIO MENEZES DE MELLO"|"ROGERIO MENEZES"|"Prefeito"|43|"PV"|"PV"|"Aguardando julgamento"|"Concorrendo"|"PDF"
"ROGÉRIO STRACIALANO PARADA"|"ROGERIO PARADA"|"Prefeito"|28|"PRTB"|"PRTB"|"Aguardando julgamento"|"Concorrendo"|"PDF"
"WILSON KELLER DE MATOS"|"WILSON MATOS"|"Prefeito"|51|"PATRIOTA"|"PATRIOTA"|"Aguardando julgamento"|"Concorrendo"|"PDF"

Fonte de dados - TSE: http://divulgacandcontas.tse.jus.br/divulga/#/municipios/2020/2030402020/62910/candidatos
Rogério Menezes recuperado em 2020-10-04: https://consultaunificadapje.tse.jus.br/#/public/resultado/0600721-68.2020.6.26.0033

## Análises
Subtração de palavras: preposições, artigos, conjunções, etc;
Lista de palavras exclu´rdas das análises: ['campinas','municipal','ser','município','ações', 'gestão','cidade','cidades','governo','pública','público','forma','todos', 'áreas','acesso','uso','sobre','número','programa','sistema','meio', 'prefeitura','secretaria','processo', 'desta']

### Nuvem de palavras (word cloud)
Nuvem de palavras de cada proposta. Quanto maior a fonte, mais ocorrências;

### Top 20 Palavras
Ranking com as 20 palavras mais comuns de cada proposta;

### Ranking por área de interesse
Com base na pesquisa do Ibope para a cidade de São Paulo realizada entre 15/09/2020 A 17/09/2020 e publicado em 21/09/2020.
Agrupamento de problemas usados na pesquisa (ver abaixo "Lista de Problemas") em temas:
- Mobilidade e zeladoria:'mobilidade','zeladoria','Trânsito','Transporte','Calçamento','ruas','avenidas','Iluminação','limpeza'
- Esporte, cultura e lazer: 'esporte','lazer','cultura','esportivas','culturais','cultural','esportiva','parque','praça','quadra'
- Saúde: 'Saúde','hospital','vida'
- Educação: 'Educação','escola','criança', 'creche'
- Segurança: 'Segurança','guarda'
- Habitação e assistência social: 'Habitação','Assistência Social'
- Trabalho e Economia: 'trabalho','Empregos','economia','empresa','imposto','taxa'
- Meio ambiente: 'Meio ambiente','ambiente','ambiental','Abastecimento','esgoto','saneamento','água'
- Corrupção e cidadania: 'Corrupção','transparência','cidadania','participativo','participativa'

Publicação: https://www.ibopeinteligencia.com/noticias-e-pesquisas/a-poucos-dias-do-inicio-da-campanha-eleitoral-celso-russomanno-esta-numericamente-a-frente-mas-tecnicamente-empatado-com-bruno-covas-na-disp/
Pesquisa: https://www.ibopeinteligencia.com/arquivos/JOB_0183_S%C3%83O%20PAULO%20-%20Relat%C3%B3rio%20de%20tabelas.pdf

#### Lista de Problemas
Pergunta: "Desta lista de áreas onde as pessoas vem enfrentando problemas de maior ou menor gravidade, por favor, diga qual é a área em que, na sua opinião, a população de São Paulo está enfrentando os maiores problemas"

- Calçamento de ruas e avenidas
- Saúde
- Educação
- Trânsito
- Transporte coletivo
- Assistência Social
- Geração de Empregos
- Iluminação pública
- Limpeza pública
- Abastecimento de água
- Segurança pública
- Habitação
- Meio ambiente
- Impostos e taxas
- Administração pública
- Atividades esportivas
- Atividades culturais
- Opções de lazer
- Rede de esgoto
- Corrupção