# testes-auto
Testes em Python usando um pouco de Selenium

Durante meu tempo estagiando na indústria, criei um desafio a mim mesmo para autoamtizar um processo que os analistas tinham que repetir todo dia.
Se trata de um KPI que era importante ao desenvolvimento da área, chamada Pendencias Ativas. Era importante acompanharem estas pendencias ativas pois era um 'engarrafamento' de material a ser liberado ao cliente. Se uma pendencia excedia mais de 2 dias, era cobrado em reunião e atrasava o atendimento ao deposito.
Esse projeto se iniciou como um site scraping no Sistema MES, uma extensão ao ERP da empresa que coleta dados de máquinas e produção, e no caso das Pendencias Ativas era escrito pelos operadores os principais motivos do material não ser liberado para o deposito. Para os analistas isso poderia ser resgatado no MES e baixado como uma planilha totalmente desestruturada.
Uma falha do sistema MES é que ele  não criava um historico das pendencias ativas, ou seja, uma vez que ela foi cocnluida, era apagada... E para uma produçao que se almeja a melhoria continua, nao ter dados sobre falhas e pontos de desenvolvimento é um grande atraso.
A proposta deste projeto foi criar esse historico, e assim pudessemos estudar quais as principais falhas que geram pendencias ativas. Assim, o programa se repetiria a cada hora: entrando no MES, filtrando inicialmente os dados para baixar e baixando; depois olharia para essa planilha nova e comparava com um data frame com os dados da ultima atualizaçao e assim se encontra 3 cenários:
1) Elementos que tem no arquivo novo e naõ no BD >>> Importar dados do novo p/ BD
2) Elementos que tem no arquivo novo e BD >>> Atualizar datas das pendencias
3) Elementos que não tem no arquivo novo e tem no BD >>> Apagar do DB (Pendencia cocnluida) e transferir para Arquivados.xlxs
Esse projeto teria capacidade de gerar 2 insights: um historico compreensível das Pendencias Ativas mais recorrentes, e facilitar um processo longo de filtragem manual dos analistas.
