# Fundamentos de Probabilidade com Python

Repositório dedicado ao estudo prático e teórico de conceitos fundamentais de probabilidade utilizando Python, `NumPy`, `SciPy` (`scipy.stats`) e `Matplotlib`. A proposta é explorar como modelar fenômenos aleatórios e observar regularidades estatísticas por meio de simulações e visualizações.

---

## Conteúdo Abordado

Os notebooks reúnem explicações teóricas, fórmulas, visualizações e exemplos práticos divididos na seguinte sequência:

1. **01 — Ensaios de Bernoulli e Distribuição Binomial** (`probabilidade1.ipynb`)

   * Modelagem de experimentos binários (sucesso/fracasso, cara/coroa) com `scipy.stats.bernoulli.rvs()`
   * Simulação de sequências de ensaios independentes e contagem de sucessos com `scipy.stats.binom.rvs()`
   * Simulação de moedas viciadas ajustando o parâmetro de probabilidade de sucesso (`p`, ex.: `p = 0.3`)
   * Diferença prática entre os parâmetros `n` (número de tentativas por rodada/bloco) e `size` (quantidade de rodadas/amostras sorteadas)
   * Reprodutibilidade de simulações com `random_state` e `numpy.random.seed()`

2. **02 — Função de Massa (PMF) e Distribuição Acumulada (CDF / SF)** (`probabilidade2.ipynb`)

   * Cálculo da probabilidade exata de $k$ sucessos em $n$ tentativas com `binom.pmf(k, n, p)`
   * Cálculo da probabilidade acumulada de até $k$ sucessos ($P(X \le k)$) com `binom.cdf(k, n, p)`
   * Cálculo da probabilidade de cauda superior ($P(X > k)$) com `binom.sf(k, n, p)` (*survival function*)

3. **03 — Valor Esperado, Média e Variância** (`probabilidade3.ipynb`)

   * Interpretação de valor esperado e variância para variáveis aleatórias discretas e para a distribuição binomial ($E(X) = np$ e $\text{Var}(X) = np(1-p)$)
   * Cálculo de estatísticas descritivas e momentos da distribuição com `scipy.stats.describe()` e `binom.stats()`
   * Ilustração prática da **Lei dos Grandes Números** com gráfico de convergência da média acumulada em lançamentos de moeda[cite: 2, 3, 4]

---

## Estrutura do Projeto

```text
.
├── probabilidade1.ipynb   # 01 - Ensaios de Bernoulli, distribuição binomial, moedas viciadas e seeds
├── probabilidade2.ipynb   # 02 - Função de massa (PMF), CDF e survival function (SF)
├── probabilidade3.ipynb   # 03 - Valor esperado, média, variância e convergência da média
├── coin-toss.gif          # Imagem ilustrativa complementar
├── expected.png           # Fórmula de valor esperado
├── variance.png           # Fórmula de variância
├── pmf.png                # Fórmula da função de massa de probabilidade
├── cdf.png                # Fórmula da função de distribuição acumulada
├── big-brain.gif          # Imagem ilustrativa complementar
└── README.md              # Documentação do repositório
```