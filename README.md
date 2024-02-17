1- Apos acessar o Microsoft Azure, clique em "criar um recurso".
2- Procure por "Machine Learning" e clique em criar.
 - na aba preencha com as seguintes informações
 - clique em criar novo e coloque um nome
 - Em Workspace coloque um nome de sua escolha
 - Region: East US
 - Store, Key, e Application deixe com o mesmo nome recomendado.
 - deixe o Container do mesmo jeito.
3- aplique em "Criar"
4- Depois clique em "Go to Resource"
5- logo apos clique em "Launch Studio"
6- Faça o seu login novamente e confirma as suas informações
7-  clique em "ML automatizado" e clique em "novo trabalho de ML automatizado"
 - Nome do trabalho: Teste de casas
 - Novo nome do experimento: Teste de casas
 - Descrição: Aprendizado de máquina automatizado para previsão preço de casas
 - Tags: nenhuma
8- E clique em avançar
 - Tipo de dados:
	- Nome: precificação
	- Descrição: Dados históricos das vendas de pizza
	- Tipo: Tabular
 - clique em Avançar
 - Clique em Arquivos da Web
	- URL da Web: https://github.com/udacity/machine-learning
	- Ignorar validação de dados: não selecione
- clique em Avnaçar e faça as seguintes configurações
 -Configurações:
 - Formato de arquivo: Delimitado
 - Delimitador: Vírgula
 - Codificação: UTF-8
 - Cabeçalhos de coluna: Somente o primeiro arquivo tem cabeçalhos
 - Pular linhas: Nenhum
 - O conjunto de dados contém dados de várias linhas: não selecione
 - clique em Avançar 2x e depois clique em Criar
9- Clique em avançar e faça as configurações conforme o seu projeto 
 	- Tipo de tarefa: Regressão
 	- Conjunto de dados: precificação
	- Coluna de destino: rentals
	- Definições de configuração adicionais:
 		- Métrica primária: NormalizeRootMeanSquaredError
 		- Explicar melhor modelo: Não selecionado
		- Use todos os modelos suportados: Não selecionado. 
		- Modelos permitidos: ReandoFront
 - Limites: expanda esta seção
	 - Máximo de tentativas: 3
	 - Máximo de tentativas simultâneas: 3
	 - Nós máximos: 3
	 - Limiar de pontuação métrica: 0,085 
 	 - Tempo limite: 15
	 - Tempo limite de iteração: 15
 	 - Habilitar rescisão antecipada: Selecionado
	 - Validação e teste:
	 - Tipo de validação: Divisão de validação de treinamento
 	 - Porcentagem de dados de validação: 10
 	 - dados de teste: Nenhum
10 - Clica em Avançar 2x e clica em "Enviar trabalho de treinamento
