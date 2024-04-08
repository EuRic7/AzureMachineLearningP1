# AzureMachineLearningP1

Para começar com o Azure Machine Learning, criei um novo espaço de trabalho no Azure Machine Learning no portal do Azure usando minhas credenciais da Microsoft. Naveguei até + Criar um recurso, procurei por Machine Learning e especifiquei a assinatura, o grupo de recursos, o nome do espaço de trabalho, a região e outras configurações conforme as instruções. Após criar o espaço de trabalho, iniciei o Azure Machine Learning studio e selecionei meu espaço de trabalho recém-criado.

Em seguida, no Azure Machine Learning studio, acessei a página Automated ML em Autoria. Criei um novo trabalho de Automated ML chamado "mslearn-bike-automl" para o tipo de tarefa de regressão, especificando os detalhes do conjunto de dados (bike-rentals) e a coluna alvo (Rentals). Configurei as configurações do trabalho, incluindo a métrica principal, os modelos permitidos (RandomForest e LightGBM) e limites para tentativas e nós.

Enviei o trabalho de treinamento e aguardei sua conclusão. Uma vez concluído, revisei o resumo do melhor modelo, selecionei o nome do algoritmo do melhor modelo para visualizar detalhes e métricas, incluindo gráficos de resíduos e predicted_true.

Após revisar o modelo, o implantei usando a opção Web service com configurações como nome, descrição, tipo de computação (Azure Container Instance) e autenticação. Testei o serviço implantado inserindo dados de exemplo na aba Teste e revisei o número previsto de aluguéis com base no modelo.
