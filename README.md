# 🤖 MACHINE LEARNING COM PYTHON - CLASSIFICAÇÃO IRIS (KERAS)

Este projeto implementa um modelo de Rede Neural Artificial (RNA) utilizando a biblioteca **TensorFlow/Keras** para classificar as três espécies de flores do renomado Iris Dataset. O foco do desenvolvimento é a padronização de dados, a otimização do modelo e a avaliação precisa de suas métricas de desempenho.

---

## 1. ⚙️ Metodologia e Desenvolvimento

### 1.1. Pré-processamento e Normalização

Antes de alimentar a Rede Neural, os dados foram tratados:
* **Codificação:** A variável alvo (espécie) foi codificada.
* **Padronização:** As características numéricas (comprimento e largura de sépalas/pétalas) foram escalonadas usando o **StandardScaler** para ter média zero e desvio padrão unitário, o que é crucial para a convergência do Keras.
* **Divisão:** Os dados foram divididos em 80% (treino) e 20% (teste) com um `random_state` para garantir a reprodutibilidade.

### 1.2. Arquitetura da Rede Neural (TensorFlow/Keras)

O modelo foi construído com a API Sequential, contendo três camadas densamente conectadas (Dense), com funções de ativação ReLU e Softmax na camada de saída. O modelo foi compilado usando o otimizador **Adam** e a função de perda `sparse_categorical_crossentropy`.

---

## 2. 📊 Resultados e Desempenho

O modelo foi avaliado no conjunto de teste, demonstrando a capacidade de generalização da Rede Neural.

### Acurácia Final

Após 10 épocas de treinamento, o modelo atingiu uma **acurácia de [INSIRA O VALOR FINAL AQUI - Ex: 86.67%]** na classificação das espécies.

### Previsão em Amostras

O desempenho foi validado em amostras de cada espécie (Setosa, Versicolor e Virginica), com o modelo prevendo corretamente cada classe com alta probabilidade.

---

## 🛠️ Tecnologias Utilizadas

* Python
* TensorFlow / Keras
* Scikit-learn (para pré-processamento)
* Pandas / NumPy