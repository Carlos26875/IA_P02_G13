# IA – Projeto 02  
## Machine Learning aplicado à Fórmula 1

**Unidade Curricular:** Inteligência Artificial  
**Ano Letivo:** 2025/2026  

### Discentes
- Carlos Sousa (24880)  
- Pedro Gonçalves (26018)  
- Carlos Moreda (26875)  

Git: https://github.com/Carlos26875/IA_P02_G13

---

## 1. Enquadramento do Projeto

Este projeto tem como objetivo aplicar diferentes técnicas de **Machine Learning** a dados históricos da Fórmula 1, utilizando o dataset público **"Formula 1 Race Data (1950–2017)"** disponibilizado no Kaggle.

Dataset original: **[Formula 1 Race Data (Kaggle)](https://www.kaggle.com/datasets/cjgdev/formula-1-race-data-19502017)**

O projeto está dividido em três notebooks independentes, mas complementares, cada um abordando um paradigma distinto de Machinig Learning:
- **Classificação supervisionada**
- **Clustering (aprendizagem não supervisionada)**
- **Regras de Associação (Apriori)**

---

## 2. Dataset

O dataset utilizado contém informação detalhada sobre corridas de Fórmula 1, incluindo pilotos, equipas, resultados, circuitos, pontos, posições de partida e classificações finais.

Principais ficheiros utilizados:
- `results.csv`
- `races.csv`
- `drivers.csv`
- `circuits.csv`
- `constructors.csv`
- `constructorResults.csv`


---

## 3. Estrutura do Projeto

O projeto está organizado nos seguintes notebooks:

### Notebook 01 – Classification
**Objetivo:**  
Prever se um piloto termina ou não no **pódio**, com base em informação disponível antes da corrida.

**Principais passos:**
- Definição do objetivo de negócio  
- Seleção e preparação dos dados  
- Criação da variável alvo (`Podium`)  
- Treino e avaliação de modelos de classificação  
- Comparação de algoritmos e métricas (Accuracy e Balanced Accuracy)  
- Ajuste de hiperparâmetros  

---

### Notebook 02 – Clustering
**Objetivo:**  
Identificar **perfis de corridas/pilotos semelhantes**.

**Principais passos:**
- Seleção de variáveis numéricas relevantes  
- Normalização dos dados  
- Aplicação do algoritmo **K-Means**  
- Determinação do número ótimo de clusters  
- Análise estatística e interpretação de cada cluster  

---

### Notebook 03 – Association Rules (Apriori)
**Objetivo:**  
Descobrir padrões frequentes e regras interpretáveis que relacionem condições de corrida com os resultados finais.

**Principais passos:**
- Transformação de cada piloto-corrida numa transação  
- Criação de itens categóricos (grid, ganhos de posição, pontos, década, tipo de equipa, resultado)  
- Aplicação do algoritmo **Apriori**  
- Ajuste dos parâmetros (`min_support`, `confidence`, `lift`)  
- Análise de regras relevantes, como:
  - partir na frente + equipa de topo = pódio  
  - partir atrás + equipa fraca = fora do Top 10  

---

## 4. Tecnologias e Bibliotecas Utilizadas

- Python  
- Jupyter Notebook  
- pandas  
- numpy  
- scikit-learn  
- mlxtend  
- matplotlib  

---

## 5. Conclusão Geral

Os três notebooks abordam o mesmo domínio (Fórmula 1) sob perspetivas diferentes e complementares:

- O **Notebook 01** foca-se em **prever** resultados (classificação);
- O **Notebook 02** foca-se em **descobrir perfis semelhantes** (clustering);
- O **Notebook 03** foca-se em **explicar padrões** através de regras interpretáveis (association rules).

Em conjunto, estes notebooks demonstram a aplicação prática de vários paradigmas de Machine Learning a um problema real.

---

## 6. Execução

Para executar os notebooks:
1. Garantir que todos os ficheiros CSV do dataset estão na mesma pasta dos notebooks;
2. Abrir os notebooks num ambiente Jupyter;
3. Executar as células pela ordem apresentada.

---