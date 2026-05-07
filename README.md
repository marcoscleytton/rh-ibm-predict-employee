# Employee Attrition Prediction | Machine Learning

##  Objetivo
Desenvolver um modelo de Machine Learning capaz de prever quais funcionários possuem maior probabilidade de deixar a empresa (**Attrition**), utilizando o dataset **IBM HR Analytics**.

---

##  Problema de Negócio
Alta rotatividade de funcionários gera:
- aumento de custos de recrutamento  
- perda de conhecimento interno  
- redução de produtividade  
- impacto em equipes e clima organizacional  

O objetivo do projeto foi criar um **modelo preditivo** para apoiar estratégias de retenção de talentos e **People Analytics**.

---

##  Dataset
- **Fonte:** IBM HR Analytics Employee Attrition Dataset  
- **Registros:** 1470 funcionários  
- **Variável target:** Attrition  
  - Yes = funcionário saiu  
  - No = funcionário permaneceu  

---

##  Tecnologias Utilizadas
- Python  
- Pandas, NumPy  
- Seaborn, Matplotlib  
- Scikit-Learn  
- XGBoost  
- Imbalanced-Learn (SMOTE)  

---

##  Etapas do Projeto

### 1. Análise Exploratória (EDA)
- Distribuição de churn  
- Correlação entre variáveis  
- Impacto de salário  
- Satisfação no trabalho  
- Work-life balance  
- Distância da empresa  
- Promoções  
- Overtime  

### 2. Pré-processamento
- Remoção de variáveis irrelevantes  
- Encoding de variáveis categóricas  
- Tratamento da variável target  
- Feature selection  
- Balanceamento com SMOTE  

### 3. Modelagem
Modelos testados:
- Logistic Regression  
- Random Forest  
- XGBoost  
- Ensemble Learning (VotingClassifier)  

---

##  Técnicas Avançadas Aplicadas
- SMOTE  
- `class_weight="balanced"`  
- Threshold Tuning  
- Precision-Recall Curve  
- ROC Curve  
- Ensemble Learning  
- Feature Importance  
- Hyperparameter Tuning  

---

##  Avaliação dos Modelos
Métricas utilizadas:
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- ROC-AUC  

---

## 🏆 Melhor Resultado
Modelo final: **Ensemble Learning (XGBoost + Random Forest + Logistic Regression)**

| Métrica   | Resultado |
| --------- | --------- |
| Accuracy  | 86%       |
| Precision | 61%       |
| Recall    | 38%       |
| F1-Score  | 47%       |
| ROC-AUC   | 0.80      |

---

##  Principais Features Identificadas
- StockOptionLevel  
- MonthlyIncome  
- JobSatisfaction  
- WorkLifeBalance  
- EnvironmentSatisfaction  
- YearsAtCompany  
- DistanceFromHome  

---

## 💡 Insights de Negócio
O projeto mostrou que:
- Remuneração influencia retenção  
- Satisfação no trabalho é um fator crítico  
- Equilíbrio entre vida pessoal e trabalho reduz churn  
- Funcionários com overtime possuem maior risco de saída  
- Distância da empresa impacta attrition  

---

## 📂 Estrutura do Projeto
```bash
project/
│
├── train_model.ipynb
├── inference.ipynb
├── ensemble_attrition_model.pkl
├── xgboost_attrition_model.pkl
├── model_columns.pkl
├── README.md
