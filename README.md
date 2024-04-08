# AzureAI900

## Resumo: 

Explorei o ML Automatizado no Azure Machine Learning para treinar e avaliar um modelo de aprendizado de máquina. Primeiro, criei um espaço de trabalho do Azure Machine Learning, em seguida, utilizei o aprendizado de máquina automatizado para treinar um modelo preditivo usando um conjunto de dados históricos de aluguel de bicicletas presente nesse link, https://aka.ms/bike-rentals. Neste repositorio, o arquivo JSON fornece informações sobre a configuração do trabalho, o tempo de execução, as métricas de desempenho do modelo e outros detalhes relevantes.

## Explorando o ML Automatizado no Azure Machine Learning

### Passos do Projeto:

1. **Criação do Espaço de Trabalho do Azure Machine Learning:**
   - Utilizei o Azure Portal para criar um novo espaço de trabalho do Azure Machine Learning.
   - Selecionei as configurações adequadas, incluindo assinatura, grupo de recursos, nome e região.

2. **Treinamento do Modelo com Aprendizado de Máquina Automatizado:**
   - Acessei o Azure Machine Learning Studio e naveguei até a página Automated ML.
   - Criei um novo trabalho de ML automatizado com as seguintes configurações:
     - Tipo de tarefa: Regressão.
     - Conjunto de dados: Histórico de aluguel de bicicletas.
     - Algoritmos permitidos: RandomForest e LightGBM.
     - Métrica primária: Raiz do Erro Quadrático Médio Normalizado.
     - Configurações adicionais, como limites de iteração e rescisão antecipada, foram especificados.

3. **Avaliação do Melhor Modelo:**
   - Após a conclusão do trabalho automatizado de aprendizado de máquina, revisei o melhor modelo treinado.
   - Analisei as métricas de desempenho, incluindo gráficos residuais e predições vs. verdadeiros.

4. **Implantação e Teste do Modelo:**
   - Implantei o modelo treinado como um serviço da Web utilizando o Azure Machine Learning.
   - Testei o serviço implantado usando dados de entrada simulados e verifiquei as previsões geradas.

### Arquivo JSON e Detalhes da Execução:

- O arquivo JSON fornecido contém informações detalhadas sobre a configuração do trabalho, o tempo de execução, as métricas de desempenho do modelo e outros detalhes relevantes.
- Ele é essencial para acompanhar e documentar o processo de treinamento e avaliação do modelo, permitindo uma análise mais aprofundada e replicação dos resultados.
