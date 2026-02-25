# Churn_TelecomX
Segundo projeto feito por mim como parte do desafio da Alura + Oracle do curso de Data Science

📊 Customer Churn Prediction | Machine Learning Project
🚀 Business Problem

Customer churn é um dos principais desafios em empresas de telecomunicação, pois impacta diretamente receita recorrente e custo de aquisição.

Este projeto tem como objetivo identificar clientes com alta probabilidade de evasão, permitindo que a empresa atue de forma preventiva com estratégias de retenção baseadas em dados.

🎯 Objetivos

- Construir um modelo preditivo para classificar clientes com risco de churn

- Identificar os principais drivers de evasão

- Garantir pipeline robusto e livre de data leakage

- Traduzir resultados técnicos em insights estratégicos

🛠️ Tech Stack

- Python

- Pandas

- NumPy

- Scikit-Learn

- Pipeline & ColumnTransformer

- Logistic Regression

- Random Forest

📂 Project Structure

```
📦 churn-prediction
 ┣ 📜 churn_model.ipynb
 ┣ 📜 requirements.txt
 ┗ 📜 README.md
```

🔍 Methodology
1️⃣ Data Preparation

- Conversão de TotalCharges para numérico

- Tratamento de valores ausentes via SimpleImputer

- Separação treino/teste com stratify

- Aplicação de StandardScaler para variáveis numéricas

- One-Hot Encoding para variáveis categóricas

2️⃣ Pipeline Construction

Todo o pré-processamento foi encapsulado em um Pipeline, garantindo:

- Reprodutibilidade

- Ausência de vazamento de dados

- Facilidade de deploy futuro

3️⃣ Model Training

Modelos avaliados:

Logistic Regression (class_weight='balanced')

Random Forest

📊 Feature Importance (Top Drivers of Churn)
- Feature	Importance
- customer_tenure	0.196
- account_Charges.Total	0.161
- account_Charges.Monthly	0.118
- internet_InternetService_Fiber optic	0.091
- account_PaymentMethod_Electronic check	0.073
- account_Contract_Two year	0.068
- account_Contract_One year	0.041
- internet_InternetService_No	0.032
- account_PaperlessBilling	0.029
- internet_TechSupport	0.028

📈 Key Insights
🔹 1. Tenure é o maior preditor de churn

Clientes nos primeiros meses apresentam maior risco de evasão.

➡ Estratégia: campanhas de retenção nos primeiros 90 dias.

🔹 2. Monthly Charges influenciam diretamente o churn

Mensalidades mais altas aumentam probabilidade de cancelamento.

➡ Estratégia: oferta de planos personalizados.

🔹 3. Contratos de longo prazo reduzem evasão

Clientes com contrato de 1 ou 2 anos possuem menor risco.

➡ Estratégia: incentivo a contratos anuais.

🔹 4. Método de pagamento impacta retenção

Pagamento via electronic check apresenta maior risco.

➡ Estratégia: incentivar débito automático.

📉 Model Evaluation

O modelo foi avaliado em conjunto de teste não balanceado para simular cenário real.

Métricas utilizadas:

1. Accuracy

2. Precision

3. Recall

4. F1-score

5. Confusion Matrix

💡 Business Impact

Com a implementação desse modelo, a empresa pode:

1. Reduzir churn com ações direcionadas

2. Diminuir CAC (Custo de Aquisição de Clientes)

3. Melhorar previsibilidade de receita

4. Priorizar clientes de alto risco

⚡ Future Improvements

1. Cross-validation

2. Hyperparameter tuning (GridSearch / RandomSearch)

3. XGBoost / LightGBM

4. SHAP values para interpretabilidade avançada

5. Deploy via API (FastAPI ou Flask)

👨‍💻 About Me

Matheus Cunha Pereira

Graduado em Análise e Desenvolvimento de Sistemas

Foco em Data Science, Machine Learning e Engenharia de Dados

🔗 Em constante evolução na área de Tecnologia e Dados

⭐ If you found this project interesting, feel free to star the repository!
