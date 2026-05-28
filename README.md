# Projeto de Mineração de Dados — Análise de Padrões Relacionados à Queda da Natalidade

Projeto desenvolvido para a disciplina de **Mineração de Dados** com o objetivo de investigar padrões relacionados à redução da natalidade no Brasil e no mundo utilizando técnicas de aprendizado não supervisionado, análise exploratória de dados e regras de associação.

O trabalho utiliza bases de dados públicas nacionais e internacionais para identificar tendências demográficas, agrupamentos regionais e associações frequentes entre características maternas, assistenciais e a redução do número de nascimentos.

---

# Objetivos do Projeto

O principal objetivo deste estudo foi analisar padrões relacionados à queda da natalidade através da aplicação de técnicas de mineração de dados em grandes bases demográficas.

Entre os principais objetivos específicos destacam-se:

* Investigar tendências globais relacionadas à redução da taxa de fecundidade e natalidade;
* Comparar padrões demográficos entre diferentes países;
* Identificar grupos de estados brasileiros com comportamentos semelhantes de natalidade;
* Aplicar algoritmos de agrupamento para detectar padrões regionais;
* Identificar associações frequentes entre características maternas e redução dos nascimentos;
* Explorar o potencial da mineração de dados na análise de fenômenos demográficos contemporâneos.

---

# Técnicas de Mineração de Dados Utilizadas

O projeto foi dividido em duas grandes etapas analíticas:

## 1. Agrupamento de Dados (Clustering)

Aplicação do algoritmo **K-Means** para identificação de grupos de estados brasileiros com padrões semelhantes de evolução da natalidade.

### Etapas realizadas:

* Pré-processamento dos dados;
* Normalização com `StandardScaler`;
* Definição do número ideal de clusters;
* Avaliação do agrupamento pelo coeficiente de silhueta;
* Análise temporal dos clusters;
* Visualização espacial dos resultados.

### Métricas utilizadas:

* Coeficiente de Silhueta;
* Método do Cotovelo (Elbow Method).

---

## 2. Regras de Associação

Aplicação do algoritmo **Apriori** para identificação de padrões frequentes relacionados à queda da natalidade.

### Variáveis analisadas:

* Escolaridade materna;
* Faixa etária da mãe;
* Número de consultas pré-natal;
* Tipo de parto;
* Redução relativa dos nascimentos.

### Métricas utilizadas:

* Suporte;
* Confiança;
* Lift.

---

# Bases de Dados Utilizadas

## Dados Internacionais

Fonte: World Bank

Foram utilizados dados demográficos internacionais entre os anos de **2000 e 2024**, permitindo comparação entre diferentes contextos populacionais e estágios de transição demográfica.

### Indicadores analisados:

* Taxa de fecundidade (`fertility rate`);
* Taxa bruta de natalidade (`birth rate`).

### Países analisados:

* Brasil
* Argentina
* Estados Unidos
* França
* Japão
* China
* Índia

---

## Dados Brasileiros

Fonte: DATASUS / SINASC

Foram utilizados dados relacionados à natalidade nos estados brasileiros entre **2000 e 2024**.

### Variáveis analisadas:

* Número de nascidos vivos;
* Idade materna;
* Escolaridade da mãe;
* Número de consultas pré-natal;
* Tipo de parto.

A análise considerou os 26 estados brasileiros e o Distrito Federal.

---

# Principais Bibliotecas Utilizadas

```python
pandas
numpy
matplotlib
scikit-learn
mlxtend
geopandas
plotly
```

---

# Estrutura do Projeto

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

```

---

# Principais Análises Realizadas

## Análise Mundial

* Evolução da taxa de fecundidade entre 2000 e 2024;
* Evolução da taxa bruta de natalidade;
* Comparação entre diferentes países;
* Visualização espacial da redução da natalidade.

---

## Agrupamento dos Estados Brasileiros

* Aplicação do algoritmo K-Means;
* Identificação de padrões regionais;
* Análise temporal da natalidade;
* Avaliação dos clusters pelo coeficiente de silhueta;
* Método do cotovelo para definição de k;
* Visualização espacial da queda dos nascimentos.

---

## Regras de Associação

* Transformação dos dados em base transacional binária;
* Aplicação do algoritmo Apriori;
* Identificação de associações frequentes;
* Relações entre:

  * escolaridade materna;
  * faixa etária da mãe;
  * pré-natal;
  * tipo de parto;
  * redução da natalidade.

---

# Exemplos de Resultados Obtidos

## Agrupamento

* Estados das regiões Sul e Sudeste apresentaram reduções mais intensas da natalidade;
* Estados das regiões Norte e Nordeste apresentaram comportamento relativamente mais estável;
* O agrupamento demonstrou padrões regionais relacionados à transição demográfica brasileira.

---

## Regras de Associação

Foram identificadas associações frequentes envolvendo:

* maior escolaridade materna;
* maior proporção de mães entre 30 e 34 anos;
* maior frequência de consultas pré-natal;
* maior ocorrência de cesarianas;
* padrões associados à redução do número de nascimentos.

---

# Como Executar o Projeto

## 1. Clonar o repositório

```bash
git clone https://github.com/nataliathomazelliferreira/mineracao_dados_natalidade.git
```

---

## 2. Instalar as dependências

```bash
pip install pandas numpy matplotlib scikit-learn mlxtend geopandas plotly
```

---

## 3. Executar os notebooks

Abra os notebooks presentes na pasta `notebooks/` utilizando Jupyter Notebook ou Visual Studio Code.

---

# Integrantes

* Natalia Thomazelli Ferreira
* Vladimir Queiroz Sejas

---

# Considerações Finais

Os resultados obtidos demonstram tendências importantes relacionadas à transição demográfica e à redução da natalidade observada no Brasil e em diferentes países ao longo das últimas décadas.

A aplicação de técnicas de mineração de dados permitiu identificar padrões regionais, agrupamentos temporais e associações frequentes entre variáveis demográficas e maternas, contribuindo para análise exploratória de fenômenos populacionais contemporâneos.

Além disso, o projeto evidencia o potencial da mineração de dados como ferramenta de apoio para estudos demográficos, análise de grandes bases públicas e compreensão de transformações sociais relacionadas à dinâmica populacional.

---

