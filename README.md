# Resumo do Projeto: Métricas de Matriz de Confusão (MNIST)

Este projeto treina uma rede neural convolucional usando TensorFlow/Keras para classificar dígitos do conjunto de dados MNIST. Após o treinamento, são calculadas e visualizadas métricas de desempenho utilizando a matriz de confusão.

## Principais etapas

- **Importação de bibliotecas**: TensorFlow, NumPy, Pandas, Seaborn, Matplotlib.
- **Carregamento e preparação dos dados**: MNIST, normalização e reshape das imagens.
- **Definição e treinamento do modelo**: Rede neural convolucional com camadas Conv2D, MaxPooling2D, Flatten e Dense.
- **Avaliação**: Predição dos rótulos de teste e cálculo da matriz de confusão.
- **Visualização**: Heatmap da matriz de confusão.
- **Cálculo das métricas**:
  - **Acurácia**: $(\frac{VP + VN}{N})$
  - **Sensibilidade (Recall)**: $(\frac{VP}{VP + FN})$
  - **Especificidade**: $(\frac{VN}{FP + VN})$
  - **Precisão**: $(\frac{VP}{VP + FP})$
  - **F-score**: $2 \times \frac{\text{Precisão} \times \text{Recall}}{\text{Precisão} + \text{Recall}}$

## Resultados

- Acurácia geral: ~99.8%
- Sensibilidade média: ~99.1%
- Especificidade média: ~99.9%
- Precisão média: ~99.1%
- F-score médio: ~99.1%

## Observações

- Todas as métricas são calculadas para cada classe e também como média geral.
- O código trata divisões por zero para evitar erros nas métricas.
- O projeto pode ser executado em ambientes Jupyter/Colab.
