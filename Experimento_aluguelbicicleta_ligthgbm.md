Configurações básicas:

Nome do trabalho: mslearn-bike-automl
Novo nome do experimento: mslearn-bike-rental
Descrição: Aprendizado de máquina automatizado para previsão de aluguel de bicicletas
Tipo de tarefa: Regressão
Dados: bike-rentals (o mesmo arquivo pois o experimento estará sendo realizado somente om o LightGBM


Configurações da tarefa:

Tipo de tarefa: Regressão
Conjunto de dados: aluguel de bicicletas
Coluna de destino: Aluguéis (inteiro)
Definições de configuração adicionais:
Métrica primária: Erro quadrático médio da raiz normalizada
Modelos permitidos: LightGBM  
Máximo de tentativas: 3
Máximo de tentativas simultâneas: 3
Nós máximos: 3
Limiar de pontuação métrica: 0,080 
Tempo limite: 15
Tempo limite de iteração: 15
Rescisão antecipada: Selecionado
Divisão de validação de treinamento
Porcentagem de dados de validação: 30
Conjunto de dados de teste: dados de teste de treinamento
teste percentual de dados: 30
Selecione o tipo de computação: Serverless
Tipo de máquina virtual: CPU
Camada de máquina virtual: Dedicado
Tamanho da máquina virtual: Standard_DS3_V2*
Número de instâncias: 1

Saída do modelo:
Saídas
Nome da saída: best_model
Modelo URL: azureml_mslearn-bike-automl_2_output_mlflow_log_model_971140291:1

Melhor resumo de modelo
Nome do algoritmo
VotingEnsemble
Detalhes do ensemble

Exibir os detalhes do ensemble
Erro de quadrado de média de raiz normalizado
0.09082
Exibir todas as outras métricas
Amostragem
100.00 %
Modelos registrados
Nenhum registro ainda
Implantar status
Nenhuma implantação ainda

Marcas
fit_time_000 : 0.060034;0.066594;1
iteration_000 : 0;1;2
pipeline_id_000 : faf12f74cf9bbd358ca5525682c5030d36f7be7c;dc4c1c986de60f33a0f8b455fff40ba23bb324c5;__AutoML_Ensemble__
predicted_cost_000 : 0;0.5;0
run_algorithm_000 : LightGBM;LightGBM;VotingEnsemble
run_preprocessor_000 : MaxAbsScaler;MaxAbsScaler;
score_000 : 0.09239622294520658;0.10175947243343658;0.09081528432277668
training_percent_000 : 100;100;100

Modelos:
NOme Algoritmo 			Erro de Quadrante 	Amostragem  Criado em 				Duração Hiperparametro
VotingEnsemble			0.09082				100.00 %	Feb 22, 2024 12:29 PM	43s		algorithm : ['LightGBM', 'LightGBM']
MaxAbsScaler, LightGBM	0.09240				100.00 %	Feb 22, 2024 12:27 PM	22s		min_data_in_leaf : 20
MaxAbsScaler, LightGBM	0.10176				100.00 %	Feb 22, 2024 12:27 PM	20s		boosting_type : gbdt


resultado do testeMétricas
explained_variance: 0.8895454
mean_absolute_error: 153.7379
mean_absolute_percentage_error: 94.29527
median_absolute_error: 114.9516
normalized_mean_absolute_error: 0.04520375

