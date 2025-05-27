# 🎗️ Análise da Sobrevida em Pacientes com Câncer de Mama

## 👩‍⚕️ Autora  
Maria Laura

## 📋 Descrição do Projeto  
Este projeto realiza uma análise estatística da sobrevida global em pacientes com câncer de mama, investigando a associação entre o estágio clínico da doença e o tempo de sobrevida. Utilizamos limpeza de dados, visualizações gráficas e modelos de sobrevivência para entender melhor os padrões da doença.

---

## 🎯 Objetivo Científico  
Investigar se o estágio clínico do câncer de mama impacta o tempo de sobrevida global dos pacientes.

### ❓ Hipóteses  
- **H₀ (Nula):** O estágio clínico não afeta a sobrevida.  
- **H₁ (Alternativa):** O estágio clínico impacta significativamente a sobrevida.

---

## 🛠️ Estrutura do Código

1. ⚙️ **Setup Inicial**: Carregamento das bibliotecas `tidyverse`, `survival` e `survminer`.  
2. 📥 **Carregamento dos Dados**: Leitura e inspeção do arquivo `clinical_data_breast_cancer.csv`.  
3. 📊 **Análise Descritiva**: Estatísticas para variáveis numéricas e categóricas.  
4. 🔄 **Manipulação dos Dados**: Conversão e recodificação das variáveis para análise.  
5. 📈 **Visualizações Exploratórias**: Boxplots e gráficos de frequência por estágio clínico.  
6. 📉 **Análise Estatística**: Teste de Levene, Kaplan-Meier e teste Log-Rank.  
7. 📝 **Conclusão**: Resultados e interpretações.

---

## 🚀 Como Executar

1. Instale o R e os pacotes necessários:  
   ```r
   install.packages(c("tidyverse", "survival", "survminer", "car"))
   ```
