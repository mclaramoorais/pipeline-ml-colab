# Pipeline de Machine Learning 

Este projeto tem como objetivo desenvolver uma pipeline de Machine Learning para detecção de fraudes em transações financeiras.

---

## 📌 Contexto

Uma instituição financeira enfrenta problemas com fraudes em transações digitais, onde pequenas operações fraudulentas conseguem passar despercebidas e gerar prejuízos.

Para resolver esse problema, foi disponibilizado um dataset com milhares de transações reais, porém anonimizado por meio de PCA (Principal Component Analysis), preservando apenas padrões estatísticos dos dados.

---

## 🔐 Sobre os dados

O conjunto de dados possui:

- V1 a V28 → variáveis transformadas por PCA  
- Time → tempo da transação  
- Amount → valor da transação  
- Class → variável alvo  

Onde:
- 0 → transação legítima  
- 1 → transação fraudulenta  

---

## ⚠️ Desafio

O dataset é altamente desbalanceado, com poucas fraudes em relação às transações normais, o que exige atenção especial na escolha das métricas e avaliação dos modelos.

---

## 🎯 Objetivo

Construir uma pipeline completa de Machine Learning para classificação de fraudes financeiras, incluindo:

- Análise exploratória dos dados  
- Pré-processamento e tratamento dos dados  
- Treinamento de modelos  
- Avaliação de desempenho  
- Interpretação dos resultados  

---

## 📊 Pontos importantes da análise

- Escolha dos algoritmos de Machine Learning  
- Avaliação com métricas adequadas (principalmente recall e precision)  
- Impacto dos erros na detecção de fraudes  
- Problemas causados pelo desbalanceamento dos dados  

---

## 🧠 Tecnologias utilizadas

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Google Colab  

---

## 📌 Observação

Projeto com foco educacional para compreensão de pipelines de Machine Learning aplicadas à detecção de fraudes.
