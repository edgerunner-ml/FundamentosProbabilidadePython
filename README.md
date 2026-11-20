# Fundamentos de Probabilidade com Python

Repositório dedicado ao estudo prático de conceitos fundamentais de probabilidade utilizando Python e a biblioteca `SciPy`. A probabilidade é a base de muitos métodos de inferência estatística e modelos em ciência de dados, permitindo compreender regularidades em fenômenos aleatórios.

---

## Conteúdo Abordado

O notebook `probabilidade1.ipynb` apresenta simulações e explicações passo a passo sobre:

1. **Ensaio de Bernoulli e Lançamento de Moedas**
   * Modelagem de experimentos com resultados binários (sucesso/fracasso, cara/coroa).
   * Geração de amostras aleatórias com `scipy.stats.bernoulli.rvs()`.
2. **Distribuição Binomial**
   * Sequência de ensaios de Bernoulli independentes.
   * Simulação de múltiplos lançamentos e contagem de sucessos utilizando `scipy.stats.binom.rvs()`.
3. **Simulação de Moedas Viciadas**
   * Alteração do parâmetro de probabilidade de sucesso (`p`) para modelar eventos assimétricos (ex.: `p = 0.3`).
4. **Reprodutibilidade com Sementes Aleatórias (*Random Seed*)**
   * Uso do parâmetro `random_state` diretamente no método `rvs()`.
   * Configuração global da semente com `numpy.random.seed()`.

---

## Estrutura do Projeto

```text
.
├── probabilidade1.ipynb   # Notebook principal com teoria, explicações e códigos em Python
├── coin-toss.gif          # Animação ilustrativa do experimento de Bernoulli
└── README.md              # Documentação do repositório
```

---

## Tecnologias e Bibliotecas

* **Python 3**
* **Jupyter Notebook / JupyterLab**
* **SciPy** (`scipy.stats`)
* **NumPy**

---

## Como Executar

1. Clone este repositório:
   ```bash
   git clone <url-do-seu-repositorio>
   cd <nome-do-repositorio>
   ```

2. Instale as dependências necessárias:
   ```bash
   pip install jupyterlab numpy scipy
   ```

3. Inicie o JupyterLab ou Jupyter Notebook e abra o arquivo `probabilidade1.ipynb`:
   ```bash
   jupyter lab
   ```

> **Nota:** Mantenha o arquivo `coin-toss.gif` no mesmo diretório do notebook `probabilidade1.ipynb` para que a animação seja renderizada corretamente nas células Markdown.