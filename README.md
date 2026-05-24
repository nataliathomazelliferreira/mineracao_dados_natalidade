# Projeto de Mineração de Dados — Análise da Queda da Natalidade

Projeto desenvolvido para a disciplina de Mineração de Dados com o objetivo de analisar padrões relacionados à queda da natalidade no Brasil e no mundo utilizando técnicas de agrupamento de dados e regras de associação.

---

## Objetivo

Investigar tendências relacionadas à redução da natalidade utilizando bases de dados reais, aplicando técnicas de mineração de dados para identificar padrões temporais, regionais e demográficos.

---

## Técnicas Utilizadas

- Análise exploratória de dados
- Pré-processamento de dados
- Clusterização com K-Means
- Avaliação de clusters com coeficiente de silhueta
- Regras de associação com algoritmo Apriori
- Visualização de dados com Matplotlib

---

## Bases de Dados

### Dados mundiais
Fonte: World Bank

- Taxa de fecundidade
- Taxa bruta de natalidade

### Dados do Brasil
Fonte: DATASUS / SINASC

- Nascidos vivos por estado
- Idade da mãe
- Escolaridade da mãe
- Consultas de pré-natal
- Tipo de parto

---

## Estrutura do Projeto

```text
Projeto-Natalidade/
│
├── README.md
├── relatorio_final.pdf
├── apresentacao.pptx
│
├── notebooks/
│   ├── 01_analise_mundial.ipynb
│   ├── 02_clusterizacao_brasil.ipynb
│   └── 03_regras_associacao.ipynb
│
├── dados/
│   ├── brasil/
│   └── mundo/
│
└── resultados/
```

---

## Principais Análises

### Análise Mundial
- Comparação da taxa de fecundidade entre países
- Evolução da taxa bruta de natalidade

### Clusterização dos Estados Brasileiros
- Identificação de grupos de estados com padrões semelhantes de natalidade
- Aplicação do algoritmo K-Means

### Regras de Associação
- Identificação de padrões relacionados à queda da natalidade
- Associação entre:
  - idade materna;
  - escolaridade;
  - pré-natal;
  - tipo de parto.

---

## Bibliotecas Utilizadas

```python
pandas
matplotlib
scikit-learn
mlxtend
```

---

## Como Executar

1. Clone o repositório:

```bash
git clone LINK_DO_REPOSITORIO
```

2. Instale as bibliotecas necessárias:

```bash
pip install pandas matplotlib scikit-learn mlxtend
```

3. Execute os notebooks na pasta `notebooks`.

---

## Integrantes

- Seu Nome
- Nome da dupla

---

## Considerações Finais

Os resultados obtidos demonstram tendências importantes relacionadas à transição demográfica e à redução da natalidade, além de evidenciar padrões demográficos associados a essas mudanças.
