# 🧬 Análise de Sobrevivência em Câncer de Mama por Estágio AJCC

Este projeto realiza uma análise estatística da associação entre o **estágio clínico do câncer de mama (AJCC Stage)** e o **tempo de sobrevida global (Overall Survival Time)**, com base em dados clínicos públicos disponibilizados no Kaggle.

---

## 🎯 Objetivo

Investigar se há uma associação estatisticamente significativa entre o **AJCC Stage** (estágio clínico do câncer) e o **tempo de sobrevida global (em meses)** de pacientes diagnosticados com câncer de mama.

---

## 📊 Hipóteses

- **Hipótese Nula (H₀):** O estágio clínico (AJCC Stage) **não** está associado a diferenças significativas no tempo de sobrevida global.
- **Hipótese Alternativa (H₁):** O estágio clínico (AJCC Stage) **está** associado a diferenças significativas no tempo de sobrevida global — ou seja, pacientes em estágios mais avançados tendem a ter menor sobrevida.

---

## 🗃️ Dataset

- **Fonte:** [Breast Cancer Proteomes - Kaggle](https://www.kaggle.com/datasets/piotrgrabo/breastcancerproteomes)
- **Arquivos utilizados:** `clinical_data.csv`
- **Variáveis de interesse:**
  - `AJCC_Stage`: Estágio clínico (I, II, III, IV)
  - `Overall_Survival_Months`: Tempo de sobrevida global (em meses)
  - `Vital_Status`: Status vital do paciente (vivo ou morto)

---

## 🧪 Metodologia

### 1. Pré-processamento
- Filtro de casos com dados completos em `AJCC_Stage` e `Overall_Survival_Months`.
- Conversão de `Vital_Status` em variável binária para eventos de sobrevivência.

### 2. Análise Estatística
- Estimativas de sobrevivência com o método de **Kaplan-Meier**.
- Teste de **log-rank** para comparar curvas de sobrevivência entre estágios.

### 3. Visualizações
- Curvas de sobrevivência por estágio (Kaplan-Meier).
- Tabela de risco ao longo do tempo.

---

## 🛠️ Tecnologias e Pacotes

- Linguagem: **R**
- Pacotes: `survival`, `survminer`, `dplyr`, `readr`
- Download automatizado do dataset via **Kaggle CLI**

---

## 📂 Estrutura do Projeto

.
├── data/
│ ├── breastcancerproteomes.zip
│ └── clinical_data.csv
├── scripts/
│ └── analise_sobrevivencia_ajcc.R
├── .gitignore
└── README.md

yaml
Copiar
Editar

---

## 📈 Resultados Esperados

A partir das curvas Kaplan-Meier e do teste log-rank, esperamos verificar uma tendência clara de menor sobrevida em estágios mais avançados, reforçando a importância do diagnóstico precoce.

---

## ✅ Como executar

1. Instale os pacotes R necessários (veja `scripts/analise_sobrevivencia_ajcc.R`)
2. Certifique-se de ter o [Kaggle CLI](https://github.com/Kaggle/kaggle-api) instalado e configurado com seu `kaggle.json`
3. Execute o script:

```r
source("scripts/analise_sobrevivencia_ajcc.R")
```