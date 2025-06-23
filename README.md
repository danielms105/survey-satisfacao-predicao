# Survey Satisfação - Predição

Este repositório contém o projeto de análise e modelagem preditiva para estimar o nível de satisfação de beneficiários a partir de dados sociodemográficos coletados em um survey.

## 📌 Objetivo

Desenvolver um modelo de machine learning capaz de prever a satisfação dos beneficiários (Baixa, Média, Alta) com base em informações como idade, renda, escolaridade, acesso a serviços, entre outras variáveis do survey.

---

## ⚙️ Tecnologias e ferramentas utilizadas

- Python (pandas, scikit-learn, imbalanced-learn, matplotlib)
- Jupyter Notebook
- Random Forest, SMOTE, RandomOverSampler, BalancedRandomForestClassifier
- GitHub

---

## 📊 Principais resultados

| Modelo                    | Acurácia | F1 macro | Recall Alta | Recall Média | Recall Baixa |
|---------------------------|----------|----------|-------------|--------------|--------------|
| Random Forest Puro         | ~50%+    | ~0.25    | ~0%         | muito baixo  | muito alto   |
| Random Forest + SMOTE      | ~49%     | ~0.33    | 6%          | 20%          | 79%          |
| Random Forest + Oversample | ~51%     | ~0.27    | 0%          | 9%           | 90%          |
| Balanced Random Forest     | ~32%     | ~0.30    | 31%         | 30%          | 34%          |

✅ **O Balanced Random Forest apresentou o melhor equilíbrio no tratamento das classes minoritárias, sacrificando acurácia para melhorar o recall de Alta e Média.**

---

## 🚀 Como executar

1️⃣ Clone o repositório:
```bash
git clone https://github.com/danielms105/survey-satisfacao-predicao.git
