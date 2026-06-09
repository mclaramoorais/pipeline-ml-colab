# Respostas da Atividade - Pipeline de Machine Learning 

**AUTORA:** Maria Clara 

---

## 1. Contexto do Problema

Uma instituição financeira enfrenta aumento de fraudes em transações digitais. O desafio não é apenas técnico — transações fraudulentas representam uma fração mínima do volume total, o que faz com que modelos tradicionais ignorem justamente os casos mais críticos.

O dataset disponibilizado contém transações reais, anonimizadas via PCA por questões de privacidade. As variáveis V1 a V28 representam combinações matemáticas dos dados originais, preservando padrões estatísticos úteis para Machine Learning sem expor informações sensíveis dos clientes.

---

## 2. Entendimento dos Dados

| Variável | Descrição |
|----------|----------|
| Time     | Tempo decorrido desde a primeira transação |
| Amount   | Valor da operação |
| Class    | 0 = legítima · 1 = fraude |

**Ponto crítico:**  
Fraudes são raras em relação ao total de transações, o que representa um risco real. Um modelo que classifica tudo como legítimo pode ter alta acurácia e ainda assim ser inútil para o negócio.

---

## 3. Decisões Técnicas e Justificativas

### Pré-processamento  
A variável **Amount** apresenta grande variação de escala e foi normalizada antes do treinamento. Isso evita que o modelo dê peso desproporcional a valores altos, distorcendo o aprendizado.

### Divisão treino/teste  
A separação dos dados garante que o modelo seja avaliado em situações que não viu durante o treinamento, simulando o comportamento real em produção.

---

## Algoritmos escolhidos

- **Regressão Logística:** Baseline interpretável, útil para entender o comportamento inicial dos dados.  
- **Random Forest:** Melhor capacidade de identificar padrões complexos e eventos raros como fraudes.

---

## Conclusão

A construção de uma pipeline eficaz para detecção de fraudes exige mais do que escolher algoritmos e gerar métricas. É necessário entender o problema de negócio, reconhecer as limitações dos dados e tomar decisões técnicas justificadas.

Neste caso, o **Random Forest** apresenta vantagem por lidar melhor com padrões complexos e dados desbalanceados.

O **Recall** guia a avaliação porque o custo de uma fraude não detectada supera o custo de um falso alarme. A acurácia, por si só, não conta a história real do modelo.
