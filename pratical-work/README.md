# 🧬 Análise de Sobrevida em Pacientes com Câncer de Mama

Este repositório apresenta uma análise estatística e visual de dados clínicos e moleculares de pacientes com câncer de mama, com ênfase em análises de sobrevivência e subtipos moleculares (PAM50). O estudo faz uso de técnicas de estatística descritiva, testes de hipóteses e visualizações, e será estendido com modelos de Kaplan-Meier e regressão de Cox.

---

## 📁 Dados

Os dados utilizados são públicos e provenientes do **Clinical Proteomic Tumor Analysis Consortium (CPTAC)**, acessados via [Kaggle - Breast Cancer Proteomes](https://www.kaggle.com/datasets/).

Arquivos principais:

- `clinical_data_breast_cancer.csv` — dados clínicos e de sobrevida
- `pam50_protein_expression.csv` — expressão de proteínas relacionadas aos subtipos PAM50

---

## 🧪 Principais Análises

- Comparação da idade entre subtipos moleculares (Luminal A, Luminal B, HER2-enriched, Basal-like)
- Análise de sobrevida por subtipo
- Associação entre estágio clínico e tempo de vida
- Exploração da relevância dos genes do painel PAM50 na distinção entre subtipos

---

## 🛠️ Como executar

### 1. Pré-requisitos

Você precisa ter o R (versão 4.0 ou superior) e RStudio instalados. Instale os pacotes necessários:

```r
install.packages(c("tidyverse", "survival", "survminer", "janitor", "car", 
                   "ggbeeswarm", "readr", "dplyr", "ggplot2", "RColorBrewer"))
```
### 2. Clonar o repositório

```bash
git clone
cd breast-cancer-survival
```
