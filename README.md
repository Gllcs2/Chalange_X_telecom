# 📊 Projeto de ETL e Análise de Evasão de Clientes – TelecomX\_BR

## 1️⃣ Visão Geral

Este projeto tem como foco principal o desenvolvimento de um pipeline de ETL (Extração, Transformação e Carga) utilizando Python, com o objetivo de compreender os principais fatores que influenciam a evasão de clientes (churn) na operadora TelecomX\_BR.

Através do consumo de dados de uma API fornecida, realizamos a limpeza, estruturação e análise exploratória para apoiar decisões estratégicas com base em evidências.

---

## 2️⃣ Objetivos do Projeto

* Construir um pipeline robusto de ETL com Python
* Identificar padrões de cancelamento de serviços (churn)
* Apoiar estratégias de retenção de clientes
* Preparar os dados para possíveis modelos preditivos no futuro

---

## 3️⃣ Ferramentas e Tecnologias

**🧪 Linguagem:**

* Python 3.x

**🔧 Principais bibliotecas utilizadas:**

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

**💻 Ambientes e ferramentas de apoio:**

* Jupyter Notebook – desenvolvimento e análise iterativa
* Git e GitHub – versionamento e colaboração
* Visual Studio Code – organização de scripts
* Scikit-learn – (em etapas futuras) para modelagem
* \[Tableau / Power BI] – opcional para visualizações mais sofisticadas

---

## 4️⃣ Estrutura do Repositório

```
Chalange_X_telecom/
├── data/
│   ├── raw/               # Dados brutos extraídos da API
│   └── processed/         # Dados tratados e prontos para análise
├── notebooks/
│   └── etl_telecomx.ipynb # Notebook principal com todo o processo de ETL e EDA
├── scripts/
│   └── etl_functions.py   # Funções auxiliares para tratamento de dados
├── README.md              # Este arquivo
├── requirements.txt       # Lista de bibliotecas utilizadas (futuramente)
└── .gitignore             # Arquivos/pastas ignoradas pelo Git
```

---

## 5️⃣ Etapas do Processo ETL

### 🔹 Extração

* Acesso direto a uma API RESTful com os dados dos clientes da TelecomX\_BR
* Armazenamento em formato `.csv` local para versionamento e reuso

### 🔹 Transformação

* Padronização de colunas e tipos de dados
* Tratamento de nulos e inconsistências
* Criação de novas variáveis derivadas (ex: faixas de tempo de contrato)
* Codificação de variáveis categóricas

### 🔹 Carga

* Salvamento dos dados processados em `data/processed`
* Pronto para análises e modelos

---

## 6️⃣ Análise Exploratória (EDA)

Durante a análise inicial, foram identificadas algumas tendências relevantes associadas ao churn, como:

| Variável           | Correlação com Churn | Observação                                       |
| ------------------ | -------------------- | ------------------------------------------------ |
| Tipo de Contrato   | 🔴 Alta              | Contratos mensais estão mais propensos ao churn  |
| Tempo de Serviço   | 🟢 Negativa          | Clientes mais antigos tendem a permanecer        |
| Faixa Etária       | 🔴 Alta              | Idosos apresentam maior taxa de cancelamento     |
| Forma de Pagamento | 🔴 Moderada          | Pagamentos automáticos estão associados ao churn |

---

## 7️⃣ Principais Conclusões

* Clientes com **contratos mensais** representam a maior parte dos cancelamentos
* A maioria dos desligamentos ocorre **nos primeiros 6 meses de contrato**
* Clientes **idosos** possuem taxas de evasão acima da média
* **Clientes de baixo valor financeiro** são os mais propensos a sair

---

## 8️⃣ Recomendações Iniciais

| Estratégia                                   | Benefício Esperado                  |
| -------------------------------------------- | ----------------------------------- |
| Incentivar contratos de longa duração        | Redução na taxa de churn            |
| Programas de fidelização para novos clientes | Maior retenção nos primeiros meses  |
| Ofertas personalizadas para idosos           | Aumento da retenção desse público   |
| Reestruturação de planos básicos             | Aumentar o ticket médio por cliente |

---

## 🔟 Autor

Gabriel Lucas
📫 Contato: gabriellcs1@hotmail.com
🔗 GitHub: [Chalange\_X\_telecom](https://github.com/Gllcs2/Chalange_X_telecom)

---


