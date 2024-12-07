# FASE-04-CTWP-Cap3

## **Descrição do Projeto**

Este projeto apresenta uma análise completa de dados de sementes, utilizando técnicas de pré-processamento, visualização e aprendizado de máquina para classificação. O objetivo foi explorar um dataset fornecido, identificar e tratar inconsistências nos dados, treinar diferentes modelos de machine learning e avaliar o desempenho de cada abordagem.

---

## **Estrutura do Código**

### 1. **Importação de Bibliotecas**
Bibliotecas utilizadas:
- `pandas`, `seaborn`, `matplotlib` para manipulação e visualização de dados.
- Modelos e ferramentas de machine learning da biblioteca `sklearn`.

### 2. **Carregamento do Dataset**
- Leitura inicial do arquivo `seeds_dataset.txt`.
- Verificação de problemas no formato dos dados, como múltiplas tabulações consecutivas.
- Correção da estrutura e geração do novo arquivo limpo chamado de `seeds_dataset_limpo.txt`.
- Adição dos títulos do arquivo e conversão para `seeds_dataset.csv`, assim podemos utilizar o pandas para a apresentação dos dados

### 3. **Análise do Dataset**
- Leitura dos tipos de informações para verificar a incoerencia ou espaços vazios.
- Verifica a presença de dados duplicados e se caso existirem, realiza a correção.
- Apresentação do gráfico para a visualização das outliers do dataset
- Verifica a distribuição de layers do modelo para entender quais modelos são interessantes de utilizar
- Apresentação da matriz de correção.

### 3. **Limpeza e Pré-processamento de Dados**
- Tratamento das outliers utilizando a mediana para substituição
- Apresentação dos dados após o tratamento

### 4. **Treinamento de Modelos**
Modelos treinados incluem:
- K-Nearest Neighbors (KNN)
- Regressão Logística
- Suporte a Vetores Máquinas (SVM)
- Árvore de Decisão
- Random Forest

### 5. **Avaliação dos Modelos**
- Métricas utilizadas para avaliação:
  - Acurácia
  - Relatório de classificação (precisão, recall e F1-score)
  - Métricas de erro como MAE, MAPE e RMSE.

---

## **Resultados Obtidos**

![image](https://github.com/user-attachments/assets/acde1a3f-7492-4f2c-9ec0-1e73fbc7ada1)

- O modelo com melhor desempenho foi `SVM (Polinomial)`, destacando-se em termos de acurácia e robustez para os três tipos de sementes
- A troca do parametro de `random_state` de 42 para 65 no processo de separação dos arquivos para treinamento e teste fez siginificantes diferenças, tornando os modelos mais eficiêntes
- A aplicação da função `MinMaxScaler` possibilitou a redução dos desvios existentes dos parametrôs, que consequentemente resultaram positivamente para a execução dos modelos
- A apresentação das métricas podemos retirar alguns insumos valiosos para entender qual modelo obteve uma melhor performance comparado a outros
  
---
