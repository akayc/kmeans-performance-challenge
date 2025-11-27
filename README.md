K-Means Clustering Challenge: Iris Dataset
-Este repositório contém a solução desenvolvida para a competição de algoritmos de Machine Learning da disciplina de Sistemas de Controle e IA.
O objetivo foi implementar e otimizar o algoritmo K-Means para agrupar dados do dataset Iris (versão não rotulada), buscando a maximização das métricas de coesão e separação dos clusters.

->Objetivo do Projeto
Realizar a clusterização não supervisionada focando nas dimensões `petal length` e `petal width`. O diferencial desta implementação é a busca exaustiva pela melhor semente de inicialização (seed), garantindo a reprodutibilidade do melhor resultado possível.

->Tecnologias Utilizadas
*Python 3
*Scikit-Learn (KMeans, StandardScaler, Silhouette Score)
*Pandas & NumPy (Manipulação de dados)
*Matplotlib (Visualização dos clusters e centroides)

->Metodologia
O código segue o seguinte pipeline:
1.  Carregamento e Limpeza: Importação do arquivo `iris_unlabeled.csv` e seleção de features.
2.  Pré-processamento: Padronização dos dados com `StandardScaler` para evitar viés de escala.
3.  Otimização de Hiperparâmetros: Loop de execução testando 200 sementes aleatórias (`random_state`) diferentes.
4.  Avaliação: Seleção do modelo com o maior Silhouette Score.
5.  Visualização: Plotagem gráfica dos clusters finais e seus respectivos centroides.

->Resultados
O algoritmo executa iterações para encontrar a configuração que maximiza o coeficiente de silhueta.
* Melhor Score alcançado: 0.6760
* Número de iterações: 1
