# Aula 2 – Métricas, Experimentos e Overfitting (Iris)

## Objetivo da aula

- Entender na prática como mudar hiperparâmetros (número de árvores da Random Forest) afeta o resultado.
- Comparar desempenho em treino e teste para ter uma noção inicial de overfitting.
- Perceber que a métrica (acurácia) varia com a forma como dividimos os dados entre treino e teste.

## Experimento 1 – n_estimators (complexidade do modelo)

Configurações testadas:

- floresta_pequena: 5 árvores → acurácia teste ≈ ...
- floresta_media: 20 árvores → acurácia teste ≈ ...
- floresta_grande: 200 árvores → acurácia teste ≈ ...

**O que percebi:**

- (escreve aqui com suas palavras)

## Experimento 2 – Treino vs Teste (overfitting básico)

- Acurácia no TREINO: ...
- Acurácia no TESTE : ...

**Reflexão:**

- (exemplo) Notei que o modelo foi bem melhor no treino que no teste, o que indica que ele se ajustou muito aos dados de treino.
- (ou) As duas acurácias ficaram parecidas, então o modelo parece generalizar bem neste problema simples.

## Experimento 3 – Tamanho do conjunto de teste (opcional)

- test_size=0.2 → acurácia ≈ ...
- test_size=0.3 → acurácia ≈ ...
- test_size=0.4 → acurácia ≈ ...

**Reflexão:**

- (exemplo) Pequenas mudanças no tamanho do conjunto de teste já mudam a acurácia.
- Isso mostra que métrica não é algo absoluto, depende da divisão dos dados.

## Conclusões da aula

- Não basta olhar para uma acurácia isolada: é preciso saber **como o modelo foi treinado e avaliado**.
- Comparar treino e teste é um passo mínimo para detectar se o modelo está “decorando” demais (overfitting).
- Mudar hiperparâmetros e repetir o experimento faz parte do trabalho normal com ML, não é desperdício: é o **processo**.
